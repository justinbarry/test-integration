FROM augurproject/dev-pop-geth as dev-pop-geth

FROM augurproject/augur-node:dev as augur-node

COPY --from=dev-pop-geth /augur.js/src/contracts/addresses.json /app/node_modules/augur.js/src/contracts/addresses.json
COPY --from=dev-pop-geth /augur.js/src/contracts/upload-block-numbers.json /app/node_modules/augur.js/src/contracts/upload-block-numbers.json

COPY wait-for-it.sh /app/wait-for-it.sh
