Ok in this file I'm chaning the inventory file yaml struction like I'm using variable at the start then applying it is same but is more profesioon way


ansible web01 -m ansible.builtin.yum -a "name=httpd state=present" --become -i inventory

ansible webservers -m ansible.builtin.service -a "name httpd state=present enabled=yes" --become -i inventory

ansible webservers -m ansible.builtin.copy -a "src=index.html dest=/var/www/html/index.html" --become -i inventory

