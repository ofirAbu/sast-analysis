# SAST analysis
In this project I'll analyze the functionality of Semgrep, codeQL and Joern on Juiceshop.


## Setting up a codeQL-DB of the Juice-Shop app
0. Install CodeQL.
1. `git clone https://github.com/juice-shop/juice-shop.git --depth 1 && cd juice-shop && npm install`
2. `mkdir ../codeqldb && codeql database create ../codeqldb --language=javascript`

## TODO List
1. Run codeQL security queries on the DB and parse paths.
2. Set up Semgrep.
3. Run Semgrep security queries on the app and parse paths.
4. Set up Joern.
5. Run Joern security queries on the app and parse paths.
6. For each service - Understand the "ease of use" of the query language" and the flexibility of the DB (expressiveness power?).
7. Run TreeSitter on the app and thoroughly analyze the output.
8. Extra: Same for AWSGoat.