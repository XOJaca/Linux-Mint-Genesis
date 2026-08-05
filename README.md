# Linux-Mint-Genesis

Linux Mint Genesis (Post-Install)

Automação do meu ambiente Linux Mint após uma instalação limpa, deixando o sistema pronto para uso prático, com minhas configurações pessoais, programas essenciais e ajustes que costumo aplicar em toda nova instalação.
Um pequeno presente para um “distro-hopper” que gosta de testar sistemas, mas quer recuperar rapidamente o ambiente familiar.


Objetivos
	Instalar programas essenciais
	Configurar aplicações automaticamente
	Aplicar personalizações do Cinnamon
	Configurar ferramentas multimídia
	Preparar ambiente para jogos
	Instalar aplicativos oficiais externos
	Economizar tempo após formatações


Requisitos
	Linux Mint instalado recentemente
	Conexão com a internet
	Usuário com permissões de administrador (sudo)


Como utilizar
Copie ou clone o projeto para o computador e execute:
chmod +x setup.sh
./setup.sh
O script principal executará todos os módulos automaticamente.



Módulos
O Genesis é dividido em módulos independentes:
Módulo	Função
01-system-update.sh	Atualização inicial do sistema
02-essential-packages.sh	Instala ferramentas básicas
03-flatpak.sh	Instala aplicações via Flatpak
04-yt-dlp.sh	Instala e configura o YT-DLP
05-cinnamon-customization.sh	Aplica tema, ícones e configurações do Cinnamon
06-network-config.sh	Configura DNS da Cloudflare
07-mpv-config.sh	Instala e configura o MPV com Vulkan
08-gaming-environment.sh	Ajustes para jogos via Proton e DXVK
09-deb-applications.sh	Instala aplicativos oficiais em formato DEB (Chrome, Brave, Steam e VS Code)

NVIDIA
Caso o sistema possua uma placa NVIDIA:
1.	Abra o Gerenciador de Drivers.
2.	Selecione a versão mais recente disponível (não necessariamente a recomendada pelo sistema).
3.	Aplique as alterações.
4.	Reinicie o computador.
Após reiniciar:
	abra o Gerenciador de Atualizações;
	atualize o sistema;
	caso as atualizações dos Flatpaks não apareçam, execute:
sudo flatpak update

Observações
Algumas configurações aplicadas pelo Genesis podem exigir uma reinicialização para funcionar corretamente.
Recomenda-se reiniciar o sistema após a execução completa do setup.

