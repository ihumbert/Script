## 因N1 刷成CoreElec系统后，权限问题存在bug，无法用默认脚本安装docker,故需要修改存储目录，由此修改了sh文件。
# host模式一键安装小雅
bash -c "$(curl https://raw.githubusercontent.com/ihumbert/Script/main/CoreElec/Alist/xiaoya.sh)" -s host

# host模式一键安装Alist tvbox
bash -c "$(curl https://raw.githubusercontent.com/ihumbert/Script/main/CoreElec/Alist/alist_tvbox_update_hostmode.sh)" -s host

# 一键安装Clouddrive
# 代理
curl -fsSL "https://raw.githubusercontent.com/ihumbert/Script/main/CoreElec/Clouddrive/clouddriveforCoreElec.sh" | bash -s install mirror

卸载命令

# 代理
curl -fsSL "https://raw.githubusercontent.com/ihumbert/Script/main/CoreElec/Clouddrive/clouddriveforCoreElec.sh" | bash -s uninstall mirror


