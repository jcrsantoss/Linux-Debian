# Linux-Debian
Minhas anotações Linux
PWD  -------------------------Diretório que estou  
LS -----------------------------Lista Arquivos e Diretórios  
LS –a------------------------- Todos os arquivos  
LS –al   ----------------------Mais informações sobre todos os arquivos 
Ld-L  -------------------------comando para listar pastas  
LS-alh ou lha --------------Informações dos Arquivos em GB. KB. TB 
LS –L (nome da pasta)---Trás o conteúdo das pastas  
Control L -------------------Atalho para limpar a tela .. 
history ----------------------Mostrar histórico de comandos  
Cat ---------------------------Visualizar os conteúdo do arquivo  
cd ../../../ ------------------Volta níveis no diretório jul 
cd -     -----------------------volta para pasta anterior 
Touch -----------------------comando para criar arquivo chat 
Touch . -----------------------Comando para criar arquivo oculto o ponto faz isso (.) 
mkdir------------------------comando para criar pastas 
rmdir-------------------------comando para remover diretórios vazios 
cat ----------------------------comando para visualizar o conteúdo de um arquivo 
rm ----------------------------comando para remover algum arquivo  
rm –r   ----------------------comando para remover diretórios  
rm-rf *  ---------------------comando para remover todos os diretórios 
cp (nome do arquivo) (nome do outro arquivo -------------- comando para copiar arquivo 
nano -------------------------comando para abrir um editor de texto  
 
Curingas  
ls a * ------------------------------usado para buscar todos os comando que começa com a letra A 
ls b* -------------------------------usada para buscar todos os comandos que começa com a letra B 
ls ?z* --------------------comando para buscar (? Uma letra aleatória) (Z letra) ( * um ou mais aleatório) 
ls m[a-c]--comando usado para buscar comando que começa com M [que tenha letra a até a letra c] 
lc m[^abc ]------------------------- comando usado para negar palavras que termina com abc  
satt 
 
Pws 
formato da impressão não compatível com a impressora 

Comandos diversos  

Df –h     ----------comando mostra o espaço livre em cada partição  
df –TH –t  (come do formato)--------Comando para buscar um modelo de arquivo especifico  

Date--------------comando para mostrar a data do sistema 
ln ----------------- comando para criar um link     

Find –name  --------------comando para pesquisar algo pelo nome  

Find \etc -mtime –1 --------comando para pesquisar arquivos alterados 1 dia atrás 

Find . -type d .name  ----------- comando para pesquisar apenas pastas 

Find . -type f .name------------- comando para pesquisar apenas arquivos 

Find  \etc -amin -10 ------------ comando para listar todos arquivos editados nos ultimos 10 minutos 

Find  \tmp -cmin –10------------comando para listar todos arquivos e pastas criados nos ultimos 10 minutos 

Find  \tmp -type f -cmin –10---comando para listar somente arquivos criado nos ultimos 10 minutos 

-cmin (último minuto) | -ctime (Último dia) |  

Less --------------- comando para pesquisar e abrir um arquivo 

Less / (nome da palavra que quer pesquisar) 
 

Sort ------------comando para listar um arquivo de forma de números para palavras de A –Z 

Sort –n     --comando para listar arquivos de A – Z e depois os números de ordem crescente 

  
Uptime---------------- comando usado para mostrar o tempo ativo da máquina desde ultimo boot 
  
dmesg -----------------comando para acessar as últimas msg do kenel  

Echo---------------------comando para exibir mensagem na tela  

Su -   --------------------------Super use (usuário administrador)touc 
Su - ----------------------------comando mais seguro para acessar super usuario 

CTL D -----------------------------comando para deixar de ser root 

sudo passwd root------------comando para alterar a senha do root 
/bin/su ------------------------Comando ideal para acessar super usuario 
Su – www-data –s /bin/bash -----------------------------comando para entrar no usuario www-data 
 
sync-------------------comando permite gravar dados da memória no sistema  

Uname –a     --------------------------comando para exibir todos os parâmetros especificado no uname 
uname –s ----------comando para exibir o kenel  
uname –n-----------vai exibir o nome da máquina na rede 
uname –r -----------vai exibir qual versão está rodando na maquina 
uname –v -----------comando para exibir a data que o kenel foi compilado  
uname –n------------ mostra a arquitetura  

 

Reboot ---------------comando usado para reiniciar a máquina somente no usuário root 

Reboot –f -----------força o reinicio da maquina a força (sempre fazer o sync semrpe que possivel antes) 

Echo b >/proc/sysrq-trigger -----------comando para reiniciar a máquina no tapa usado para modo de emergência  

Halt ----------comando para desligar a maquina 
shutdown –h now ----------comando para para desligar a máquina tbm 
echo 0 >/roc/sysrq-trigger------------comando para desligar a máquina forçado para emergência  

Shutdown –h 09:40 ---------------Exemplo de comando para desligar a máquina com horário agendado  Shutdown –c --------------------comando para cancelar o agendamento de desligamento da maquina  

 
 
lsattr-----------------------comando para vefiria os atributos dos arquivos ou pasta  

 Chattr ---------------------comando usado para alterar atributo e diretorios  
Chattr +i (nome do arquivo) ------------------Comando adicionar  um atributo ao arquivo deixando imutável, sem permissão para alteração.  
chattr –i --------------------C 

omando para remover um atributo de algum arquivo  

Cmp ------------------ Compara dois arquivos de qualquer tipo (binário ou texto). 
 
 

Wich(nome do binario) -------------------comando usado para mostrar aonde o binário se encontra  

 

Mcedit/caminho/arquivo------------------Comando para abrir algum arquivo com o editor 
apt-get install mc ---------------------------Comando para instalar o mcedit caso não tenha 

ps -a    ------------------------------------------Comando para mostrar o que está rodando em todos terminais  

 

 

Alt F2 ----------------------------comando para abrir outro terminal 
apt install screen--------------Comando para instalar multiplos terminais   
screen---------------------------------------comando para dar inicio a uma screen 
CTL + A +C ----------------------------------para abrir uma nova screen 
CTL + A + W -----------------------------para visualizar quantas screen estão abertos 
CLT + A + 1, CLT + A + 2, CLT + A + 0 ------------comandos para navergar entre as escreen  
CLT + D -------------------------------------------------comando para fechar uma screen 
CLT –X -------------------------------------------------comando para abrir uma screen 

 
Instalação e Configuração da Interface Gráfica: 

Bem, nosso primeiro passo será atualizar a lista de repositórios: 
# apt-get update 

 
 
O primeiro componente que iremos instalar é o  X Window System: 
# apt-get install x-window-system 

 

Agora que temos o X Window System instalado, podemos instalar Gerenciadores de Janelas e Ambientes de Desktop. Há vários disponíveis, como o gnome, icewm, xfce4, kde, fluxbox, etc.; nesta demonstração, iremos instalar o GNOME: 
# apt-get install gnome 

cat /etc/os-release ---------------comando para verificar a versão do linux 

Após a instalação finalizar, vamos testar a interface gráfica iniciando-a a partir do console com o comando startx:: 

# startx 

 

 
