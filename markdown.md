# caminhada


"git status" serve para mostar status dos argivos <br/>
"git add "aquivo" adiciona o arquivo na grade<br/>
" git add ." adiciona varios arquivos de uma vez<br/>
"git restore --staged <file>..." restalrar estado<br/>
  <br/>
  # Atividade troca de nome.<br/>
  <br/>
  "hostname" indentificar o nome da macna<br/>
  "hostnamectl" dados do pc<br/>
  "hostnamectl set-hostname .novo nome do pc" mudar o nome do pc<br/>
  apos altere o arquivo "sudo nano /etc/hosts" onde estiver o antigo nome colocar o novo.<br/>
  teste com "hostname"<br/>
  apos desloge e reloge<br?>
  
  outra maneira
  
  sed 's/NOME-VELHO/NOME-NOVO/'  /etc/hosts
Para valer
sudo sed -i 's/NOME-VELHO/NOME-NOVO/'  /etc/hosts
  
  # Atividade troca de ips
  
  ##Com relação a interfaces de rede, é importante saber:
Listar as interfaces de rede reconhecidas pelo sistema operacional
  "ip -br -c a"
  "ip link" co
  "ip -br -c link"
  
## Saber ativar ou desativar uma interface de rede
  "sudo ip link set -interface- up" sobe a iterface
  "sudo ip link set -interface- down" deruba a iterface
  
  
## Configurar uma interface de rede com endereço IP dinâmico (DHCP) ou estático
1. edite "sudo nano /etc/netplan/00-installer-config.yaml"
  
  No nano, CTRL+K apaga a linha atual
  
2. Salvar o arquivo
  
netplan apply
ip -br -4 a
  
ip dinamico:
ethernets:
  enp0s8:
    dhcp4: true
  ip statc:
  
  
  
Configurar máscara de sub rede
Configurar endereço(s) IP de servidor(es) DNS a serem consultados
Configurar endereço IP do roteador padrão
