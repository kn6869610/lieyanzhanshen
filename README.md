# �P�K�ԯ� �~��
(�P�K�ԯ��B�P���ԯ�?  �~���о�)

�A�Ⱥݸ̥i�঳SecurityBox�BGameServer�BLoginServer

##�~���覡
�s�� wwwroot\game1.php �M���H�U�϶�
<pre><code>
  function getParams()
		{
			return "http://127.0.0.1/?server_ip=�A���A�Ⱦ�IP&server_port=9001&pass_user_name=<?=$user?>&encrypted_string=<?=$password?>&server_id=test_1&source=0&sub_source=&flags=4&time=1392385580&agent=9377&server=292&is_client=true";
		}
</code></pre>


�s�� Server\GameServer\conf\realms.conf 
	<LogonServer Address = "127.0.0.1" Port = "9555" Name = "Default Logon" RealmCount = "1">
	<MonitorServer Address = "0.0.0.0" Port = "18800" Enable = "0">
	<WorldDatabase Hostname = "127.0.0.1" Username = "root" Password = "123456" Name = "game" Port = "3306">

	<Realm1 Name = "test_1"
		Address = "�A���A�Ⱦ�IP:10009" 
		Icon = "PVP"
		Population = "1.0"
		TimeZone = "1">
		
�����W�z��B�J�Y�i�~��
