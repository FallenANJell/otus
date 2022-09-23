#Установка и натйрока веб сервера

#утсановка nginx
sudo yum -y install epel-release
sudo yum -y install nginx

#перенсти конфиг в /etc/nginx/conf.d

sudo systemctl start nginx
sudo systemctl enable nginx

#установка apach
sudo yum -y install httpd
#перенсти конфиг в /etc/httpd/conf/httpd.conf
#скопировать стартовые страницы в /var/www/html
#првоерка конфига 
sudo httpd -t
sudo systemctl start httpd
sudo systemctl enable httpd

