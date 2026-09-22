# ingestion data

- Dowmload the dataset from 'data\source\data.txt'
- create and EC2 instance > docker container > mcr.microsoft.com/mssql/server:2022-latest
- spin up the legacy MSSQL server
'''
docker run -e "ACCEPT_EULA=Y"
 -e "MSSQL_SA_PASSWORD=Password123!"
 -p 1433:1433
 --name legacy-mssql
 -d my-mssql-image

'''

- install the req: pip install -r requirements.txt