ssdkktes 2t another test22121sdsds2
sdsdasdjbjsdfsdsfdssdsdsdsdsasdssdssdsdfsdfsdsdfdגכגגככגbhvhdfגכגעכע
שדש

 /xray/api/v1/packages?order_by=&package_type=rpm


 POST -X uadmin:Password1! http://172.16.12.226/xray/api/v1/ignore_rules
 -d
{
  "notes": "Ignore common Alpine components",
  "ignore_filters": {
    "vulnerabilities": ["any"],
    "licenses": ["any"],
    "cves": ["any"],
    "components": [
      { "name": "3.10:libssl1.1:1.1.1k-r0" }
    ]
  }
}


shared:
  database:
    type: postgresql
    driver: org.postgresql.Driver
    url: jdbc:postgresql://127.0.0.1:5432/xraydb
    user: xray
  
    password: "password"
