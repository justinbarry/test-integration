FROM augurproject/dev-pop-geth as dev-pop-geth

FROM augurproject/augur:dev

COPY env.json /augur/build/config/env.json

COPY --from=dev-pop-geth /augur.js/src/contracts/addresses.json /augur/node_modules/augur.js/src/contracts/addresses.json
COPY --from=dev-pop-geth /augur.js/src/contracts/upload-block-numbers.json /augur/node_modules/augur.js/src/contracts/upload-block-numbers.json
