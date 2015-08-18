# 烈焰戰神 外網
(烈焰戰神、烈火戰神?  外網教學)

服務端裡可能有SecurityBox、GameServer、LoginServer

##外網方式
編輯 wwwroot\game1.php 尋找到以下區塊
<pre><code>
  function getParams()
		{
			return "http://127.0.0.1/?server_ip=你的服務器IP&server_port=9001&pass_user_name=<?=$user?>&encrypted_string=<?=$password?>&server_id=test_1&source=0&sub_source=&flags=4&time=1392385580&agent=9377&server=292&is_client=true";
		}
</code></pre>


編輯 Server\GameServer\conf\realms.conf 
	<LogonServer Address = "127.0.0.1" Port = "9555" Name = "Default Logon" RealmCount = "1">
	<MonitorServer Address = "0.0.0.0" Port = "18800" Enable = "0">
	<WorldDatabase Hostname = "127.0.0.1" Username = "root" Password = "123456" Name = "game" Port = "3306">

	<Realm1 Name = "test_1"
		Address = "你的服務器IP:10009" 
		Icon = "PVP"
		Population = "1.0"
		TimeZone = "1">
		
完成上述兩步驟即可外網
