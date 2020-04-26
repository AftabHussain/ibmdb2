About IBM DB2 Warehouse - [*](https://www.ibm.com/support/knowledgecenter/SSCJDQ/com.ibm.swg.im.dashdb.doc/local_overview.html)

About Catalog Views, first 2 bullets - [*](https://www.ibm.com/support/knowledgecenter/SSCJDQ/com.ibm.swg.im.dashdb.sql.ref.doc/doc/r0008443.html)

Database Catalog - "The database catalog of a database instance consists of metadata in which definitions of 
database objects such as base tables, views (virtual tables), synonyms, value ranges, indexes, 
users, and user groups are stored." - [*](https://en.wikipedia.org/wiki/Database_catalog)

Base table - "A base table is a physical structure that contains stored records. This structure can have any physical 
format as long as it can be presented to the user as a collection of rows and columns." - [*](https://kbs.custhelp.com/app/answers/detail/a_id/289/~/what-is-a-base-table%3F)

SYSCAT.TABLES catalog view - [*](https://www.ibm.com/support/knowledgecenter/SSCJDQ/com.ibm.swg.im.dashdb.sql.ref.doc/doc/r0001063.html)

________

Connecting to a IBM DB2 Database on the IBM Cloud using connection strings via sql 
in a python interpreter (This setup was done from the JupyterLab environment, in the IBM Skills Network Labs Platform):
```python
#%sql ibm_db_sa://my-username:my-password@my-hostname:my-port/my-db-name
%sql ibm_db_sa://xxxxxx:xxxxx@dashdb-txn-sbox-yp-dal09-03.services.dal.bluemix.net:50000/BLUDB
```

Here's how you can obtain the connection string - From your IBM Cloud Dashboard, go to your IBM Db2 Service. Then go to 
Service Credentials and then expand a service credential view. You should see several entries. The connection string 
is in the entry `uri:`.
