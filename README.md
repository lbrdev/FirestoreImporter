# DB Importer
## How to use
0. Add web project configuration in Firebase console. Generate configuration and replace in `config.js`. Open settings and create service account, download configuration and replace in `serviceAccount.json`.
1. Convert  `.csv` file into `JSON` using this link - ([CSV to JSON - CSVJSON](https://www.csvjson.com/csv2json))
2. Copy `JSON` data into file (`example.json`).
3. Save file
4. Check access rules at **Firestore**. If collection that you need to update has `allow read: if request.auth.uid != null` change it to `allow read, write` and publish. ~Don't forget to revert it back.~
5. Delete collection in **Firestore**
6. Open terminal and run
```
node import_*collection*.js
```

# Contacts
lbrdev.contact@gmail.com
