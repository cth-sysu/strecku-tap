# strecku-tap

Command-line binary used with strecku store credentials as a kiosk interface.

## buy

Script that reads 1 scanned code (RFID or BAR-code reader) and;

1) if associated with user, buys 1 more of the most recently purchased product
2) if product bar code, prints the product name to stdout
3) if unknown code, associates the code to the most recent buyer of the store

## loop

Wraps `buy` in a loop.

## How to run

Put raw store credentials in a `token` file, then run `$ ./loop`.
