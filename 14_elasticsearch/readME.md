To launch elastic search do this:

PS C:\Users\reegauta\Documents\Simplon_projects> cd ..
PS C:\Users\reegauta\Documents> cd ..
PS C:\Users\reegauta> cd .\Downloads
PS C:\Users\reegauta\Downloads> cd .\elasticsearch-7.11.2
PS C:\Users\reegauta\Downloads\elasticsearch-7.11.2> .\bin\elasticsearch.bat

To launch Kibana do this:

PS C:\Users\reegauta\Documents\Simplon_projects> cd ..
PS C:\Users\reegauta\Documents> cd ..
PS C:\Users\reegauta> cd .\Downloads
PS C:\Users\reegauta\Downloads> cd .\kibana-7.11.2
PS C:\Users\reegauta\Downloads\kibana-7.11.2> .\bin\kibana.bat

Commads in cmd to quickcheck and bulk update and check my indices:

bulk update with existing json file:

- $response = Invoke-RestMethod -Method POST -Uri "http://localhost:9200/_bulk" -Headers $headers -InFile "movies_elastic.json"
- $response | ConvertTo-Json -Depth 10
- Invoke-RestMethod -Method GET -Uri "http://localhost:9200/_cat/indices?v"

# Create the movies2 index with your mapping

$mappingJson = Get-Content -Raw -Path "mapping.json"
Invoke-RestMethod -Method PUT -Uri "http://localhost:9200/movies2" -Headers @{"Content-Type" = "application/json"} -Body $mappingJson

# Then check if it was created

Invoke-RestMethod -Method GET -Uri "http://localhost:9200/_cat/indices?v"
