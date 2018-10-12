# access-注入
## access数据库的后缀名
`.mdb`
## access配置文件
`Driver={"microsoft access driver(*.mdb); dbq=*.mdb;uid=admin;pwd=pass;"}` \
`dim conn` \
`set conn = server.createobject("adodb.connection")` \
`conn.open "provider=Microsoft.ACE.OLEDB.12.0;" & "datasource = " & server.mappath("bbs.mdb")`
