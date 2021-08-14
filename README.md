# Install_SNGREP
Instalação do SNGREP


CentOS / Fedora / RHEL
Você pode usar os repositórios Irontec para algumas versões do CentOS (5,6,7,8), Fedora (20,21) e Red Hat (5,6,7,8).
Binários são construídos apenas para arquiteturas amd64 e i386 sem suporte SSL.

Adicione as informações do repositório Irontec a /etc/yum.repos.d/irontec.repo

Para Centos:

[irontec] 
name = Irontec RPMs repository 
baseurl = http: //packages.irontec.com/centos/$releasever/$basearch/
Para Fedora:

[irontec] 
name = Irontec RPMs repository 
baseurl = http: //packages.irontec.com/fedora/$releasever/$basearch/
Para Red Hat Enterprise Linux:

[irontec] 
name = Irontec RPMs repository 
baseurl = http: //packages.irontec.com/rhel/$releasever/$basearch/
Adicionar chave pública de repositórios Irontec:

rpm --import http://packages.irontec.com/public.key
E instale o pacote

yum install sngrep
Se você encontrar problemas de instalação devido a erros de gpg, tente

yum --nogpgcheck install sngrep

