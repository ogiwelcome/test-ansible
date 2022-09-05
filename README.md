## こんにちは
- ansibleで遊んでいます
- ipは適当にその時作ったものを埋め込んでいるので適宜変えてください
## 必要なパッケージ
- create_ec2
  - boto3
## 権限
- aws.pem(ec2で作るキーペア)の権限によってはToo Openとか言われる、600推奨？
## コマンドメモ
- ping送る
```
ansible -i ./nginx_setup/inventory.ini server -m ping
```
- playbook使う
```
ansible-playbook -i ./nginx_setup/inventory.ini ./nginx_setup/playbook.yml
```