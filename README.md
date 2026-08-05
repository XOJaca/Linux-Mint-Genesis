# Linux Mint Genesis (Post-Install)

Automação do meu ambiente Linux Mint após uma instalação limpa, deixando o sistema mais bonito e pronto para uso com alguns programas, configurações e personalizações favoritas.

Um pequeno presente para qualquer **distro-hopper** como eu que sempre que puder, ter a possibilidade de voltar para o Linux Mint já pronto, mas não gosta de repetir sempre alguns dos mesmos processos de instalação e configuração.

---

# ✨ Recursos

O Linux Mint Genesis automatiza diversas tarefas realizadas após uma instalação limpa do sistema.

Atualmente ele é capaz de:

* 📦 Atualizar completamente o sistema
* 🛠️ Instalar programas essenciais em Debian e em Flatpak
* 🎬 Instalar e configurar o YT-DLP
* 🎨 Aplicar tema, ícones e configurações personalizadas do Cinnamon
* 🌐 Configurar automaticamente o DNS da Cloudflare
* 🎥 Instalar e configurar o MPV utilizando Vulkan (Assim tendo Suporte a usar o LSFG-VK no MPV + Legendas Amarelas)
* 🎮 Preparar o ambiente para jogos via Proton e DXVK
* 💻 Instalar Google Chrome, Brave, Steam e Visual Studio Code

---

# 📂 Estrutura do Projeto

```text
Linux Mint Genesis (Post-Install)
├── configs/
│   ├── cinnamon/
│   ├── icons/
│   └── themes/
├── modules/
│   ├── 01-system-update.sh
│   ├── 02-essential-packages.sh
│   ├── 03-flatpak.sh
│   ├── 04-yt-dlp.sh
│   ├── 05-cinnamon-customization.sh
│   ├── 06-network-config.sh
│   ├── 07-mpv-config.sh
│   ├── 08-gaming-environment.sh
│   └── 09-deb-applications.sh
├── setup.sh
├── VERSION
└── README.md
```

---

# 📋 Requisitos

* Linux Mint instalado recentemente
* Conexão com a internet
* Usuário com permissões de administrador (`sudo`)
* Arquitetura **amd64 (x86_64)**

---

# 🚀 Como utilizar

1. Baixe a versão mais recente do **Linux Mint Genesis** na seção **Releases** deste repositório.
2. Extraia o arquivo `.zip` em qualquer pasta de sua preferência.
3. Abra a pasta extraída.
4. Clique com o botão direito em `setup.sh` e escolha **Abrir no Terminal**

4.2. Caso não tenha essa opção, então aperte com o botão direito do mouse na pasta baixada e aperte em "Abrir no Terminal"
Execute então o seguinte código:

```bash
./setup.sh
```

O Genesis executará automaticamente todos os módulos na ordem correta.

> Durante a execução será solicitada a senha do usuário (`sudo`) para instalar programas e aplicar configurações no sistema.

---

# 📦 Módulos

| Módulo                         | Função                                                   |
| ------------------------------ | -------------------------------------------------------- |
| `01-system-update.sh`          | Atualiza o sistema e seus pacotes                        |
| `02-essential-packages.sh`     | Instala programas e dependências essenciais              |
| `03-flatpak.sh`                | Configura o Flatpak e instala aplicações                 |
| `04-yt-dlp.sh`                 | Instala e configura o YT-DLP                             |
| `05-cinnamon-customization.sh` | Aplica tema, ícones e configurações do Cinnamon          |
| `06-network-config.sh`         | Configura automaticamente o DNS da Cloudflare            |
| `07-mpv-config.sh`             | Instala e configura o MPV utilizando Vulkan              |
| `08-gaming-environment.sh`     | Configura o ambiente para Proton e DXVK                  |
| `09-deb-applications.sh`       | Instala Google Chrome, Brave, Steam e Visual Studio Code |

---

# 🎮 NVIDIA

Caso o computador utilize uma placa de vídeo NVIDIA, recomenda-se realizar os seguintes passos após a execução do Genesis:

1. Abra o **Gerenciador de Drivers**.
2. Selecione a versão mais recente disponível (não necessariamente a recomendada).
3. Aplique as alterações.
4. Reinicie o computador.

Após reiniciar, abra o **Gerenciador de Atualizações** e instale todas as atualizações disponíveis.

Caso as atualizações dos aplicativos Flatpak não apareçam, execute:

```bash
sudo flatpak update
```

---

# ⚠️ Observações

* Algumas configurações podem exigir uma reinicialização para serem aplicadas corretamente.
* O projeto foi desenvolvido e testado para o **Linux Mint Cinnamon**.
* Os módulos podem ser executados individualmente, caso seja necessário.

---

# 📄 Licença

Este projeto é disponibilizado gratuitamente para uso pessoal e aprendizado. Sinta-se à vontade para estudar, modificar e adaptar o código conforme suas necessidades.
