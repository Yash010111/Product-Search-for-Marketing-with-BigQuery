# Product-Search-for-Marketing-with-BigQuery

## Skills Boost Arcade Base Camp September 2025:Product Search for Marketing with BigQuery



### ⚠️ Disclaimer
- **This script and guide are provided for  the educational purposes to help you understand the lab services and boost your career. Before using the script, please open and review it to familiarize yourself with Google Cloud services. Ensure that you follow 'Qwiklabs' terms of service and YouTube’s community guidelines. The goal is to enhance your learning experience, not to bypass it.**

### ©Credit
- **DM for credit or removal request (no copyright intended) ©All rights and credits for the original content belong to Google Cloud [Google Cloud Skill Boost website](https://www.cloudskillsboost.google/)** 🙏


ACCURATE COMMANDS
USE FOLLOWING COMMAND 

## STEP 1: IMPORT CSV

MAKE SURE TO REPLACE BUCKET NAME ACCORDING TO LAB INSTRUCTIONS
```
bq load --source_format=CSV --skip_leading_rows=1 --autodetect products.products_information gs://YOUR_BUCKET_NAME/products.csv
```

EXAMPLE:
```
bq load --source_format=CSV --skip_leading_rows=1 --autodetect products.products_information gs://qwiklabs-gcp-03-0a2611318019-bucket/products.csv
```
## STEP 2: Create a search index

```
bq query --use_legacy_sql=false 'CREATE SEARCH INDEX products_information_index ON products.products_information(ALL COLUMNS)'
```
## STEP 3: Run the search index

```
bq query --use_legacy_sql=false 'SELECT * FROM products.products_information WHERE SEARCH(products_information, "22 oz Water Bottle")'
```
### Congratulations !!!!

### IF NOT WORKING KINDLY INFORM VIA DM
```
+91 9371574317
```

### CONNECT WITH INSTAGRAM AND LINKEDIN
<a href="https://www.instagram.com/yash.paraskar0208/" target="_blank" style="text-decoration: none;">
  <img src="https://img.shields.io/badge/-Follow_Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white&labelColor=E4405F&color=white&gradient=linear-gradient(90deg, #E4405F, #C13584)" alt="Instagram"/>
</a>
<a href="https://www.instagram.com/drabhishek.5460/" target="_blank" style="text-decoration: none;">
  <img src="https://tse2.mm.bing.net/th/id/OIP.Idv3um5LvEcT7k_MjNNpoQHaCd?r=0&w=729&h=242&rs=1&pid=ImgDetMain&o=7&rm=3?style=for-the-badge&logo=instagram&logoColor=white&labelColor=E4405F&color=white&gradient=linear-gradient(90deg, #E4405F, #C13584)" alt="Linkedin" width="100" height="100"/>
</a>
