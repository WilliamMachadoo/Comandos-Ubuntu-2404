# Comandos-Ubuntu-2404
Observações: comando sudo concede privilégio de administrador<br> 
apt: gerenciador de pacotes<br>
 
**sudo apt update**: Verifica se há versões novas dos programas que você pode instalar ou já tem no sistema.<br>
- Atualiza a lista de pacotes disponíveis no repositório.<br>
  - Exemplo: como dar uma olhada no “catálogo” mais recente de aplicativos e atualizações antes de instalar algo.<br>
 
**sudo apt upgrade**: Serve para instalar as versões mais recentes dos programas que você já usa.<br>
- Atualiza os pacotes que já estão instalados no sistema.
  - Exemplo: como utilizar os aplicativos do seu celular – só que aqui, no Linux.<br>
 
**sudo reboot**: Reinicia o computador.
- Serve para aplicar certas atualizações, corrigir erros ou reiniciar o sistema de forma segura.
  - Exemplo: é o famoso “desliga e liga de novo” para o computador.<br>
 
**sudo apt install build-essential dkms linux-headers-$(uname -r)** 
- Instala: build-essential: ferramenta para compilar código-fonte<br>
  - dkms: recompilador de aplicações para compatibilidade com Kernel do convidado (guest) <br>

**cd /media/$USER/VBox_GAs_7.0.6**<br>
 - Caminha até o diretório onde está o aplicativo para instalar recursos adicionais de convidado 
  - $USER é uma variável de ambiente que referência o valor do usuário que está logado (nome de usuário)<br>
 
**sudo ./VBoxLinuxAdditions.run**
Executa a aplicação disponível no diretório que acessou e instala os recursos<br>
 
**lsmod | grep vbox lsmod**: 
- Lista módulos carregados no Kernel 
  - grep: funciona como um filtro para pesquisar apenas as linhas que contenham o texto que deseja pesquisar (nesse caso, vbox) 
vbox: prefixo que inicia normalmente os nomes dos módulos do VirtualBox
