# 因N1 刷成CoreElec系统后，权限存在bug，无法用默认脚本安装docker,故需要修改存储目录，由此修改了sh文件。
## host模式一键安装小雅
bash -c "$(curl https://raw.githubusercontent.com/ihumbert/Script/main/CoreElec/Alist/xiaoya.sh)" -s host

## host模式一键安装Alist–tvbox
bash -c "$(curl https://raw.githubusercontent.com/ihumbert/Script/main/CoreElec/Alist/alist_tvbox_update_hostmode.sh)" -s host

## 一键安装卸载Clouddrive
## 安装命令
curl -fsSL "https://raw.githubusercontent.com/ihumbert/Script/main/CoreElec/Clouddrive/clouddriveforCoreElec.sh" | bash -s install mirror

## 卸载命令
curl -fsSL "https://raw.githubusercontent.com/ihumbert/Script/main/CoreElec/Clouddrive/clouddriveforCoreElec.sh" | bash -s uninstall mirror

## 安装portainer-ce中文版
docker run -d --restart=always --name="portainer" -p 9000:9000 -v /var/run/docker.sock:/var/run/docker.sock 6053537/portainer-ce



