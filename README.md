[⬅Voltar](https://memorise-codigos.github.io)
# Linguagem zsh para terminal
A Zsh (Z shell) é uma poderosa shell de linha de comando que oferece muitos recursos e personalizações em comparação com as shells padrão, como Bash e Tcsh. A Zsh está disponível no Linux e no macOS por padrão e é altamente personalizável e extensível por meio de plugins e temas. Neste manual, forneceremos uma visão geral dos recursos básicos da Zsh e como usá-la efetivamente.
## Instalação
No Linux, a Zsh geralmente já está instalada por padrão. No macOS, ela também vem pré-instalada, mas em versões mais antigas do sistema operacional pode ser necessário instalá-la manualmente. Você pode verificar se a Zsh está instalada em seu sistema executando o seguinte comando em um terminal:
- `zsh --version`

Se a Zsh estiver instalada, você verá a versão da Zsh que está sendo executada. Caso contrário, você pode instalá-la com um gerenciador de pacotes como o Homebrew (no macOS) ou o apt-get (no Linux).
## Configuração
A Zsh é altamente personalizável por meio de seu arquivo de configuração principal, que é chamado de .zshrc. Este arquivo é executado sempre que a Zsh é iniciada e contém várias configurações e definições de alias que você pode personalizar de acordo com suas necessidades.

Você pode criar ou editar o arquivo .zshrc com um editor de texto como o Nano ou o Vim. Por exemplo, para editar o arquivo .zshrc usando o Nano, execute o seguinte comando em um terminal:
- `nano ~/.zshrc`

Isso abrirá o arquivo .zshrc no editor de texto Nano, permitindo que você adicione ou edite as configurações.
## Recursos básicos
A Zsh oferece muitos recursos úteis que podem ajudar a tornar a linha de comando mais eficiente e fácil de usar. Aqui estão alguns recursos básicos que você pode começar a usar:
### Auto-completar
Um dos recursos mais úteis da Zsh é o auto-completar. Quando você digita o começo de um comando, caminho ou arquivo e pressiona a tecla Tab, a Zsh tenta completar o restante automaticamente. Isso pode economizar muito tempo, especialmente quando você está digitando um caminho ou arquivo longo.
### Histórico de comandos
A Zsh mantém um histórico de todos os comandos que você digitou. Você pode acessar o histórico digitando o comando history em um terminal. Além disso, você pode navegar pelo histórico de comandos usando as teclas de seta para cima e para baixo.
### Aliases
Os aliases permitem que você crie atalhos para comandos mais longos ou complexos. Por exemplo, você pode criar um alias para o comando ls -la digitando o seguinte comando:
- `alias ll='ls -la'`

Assim, sempre que você digitar ll no terminal, a Zsh executará o comando ls -la.
## Prompt personalizado
Você pode personalizar o prompt da Zsh para exibir informações adicionais, como o diretório atual, o nome do usuário e a hora atual. Você pode fazer isso editando o arquivo .zshrc e definindo a variável PS1. Por exemplo, para exibir o diretório atual no prompt, você pode definir a variável PS1 como:
- `PS1='%n@%m:%~$'`

Isso exibirá o nome do usuário (%n), o nome do computador (%m) e o diretório atual (%~) no prompt. O sinal de dólar ($) indica o final do prompt.
## Plugins e temas
Além dos recursos básicos, a Zsh também pode ser estendida com plugins e temas. Os plugins adicionam novos recursos e funcionalidades à Zsh, enquanto os temas mudam a aparência do prompt e adicionam recursos visuais.

Você pode instalar plugins e temas usando um gerenciador de pacotes como o Oh My Zsh, que é um framework de gerenciamento de configurações para a Zsh. O Oh My Zsh torna mais fácil instalar e gerenciar plugins e temas, e também vem com vários plugins e temas populares pré-instalados.

Para instalar o Oh My Zsh, execute o seguinte comando em um terminal:
- `sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`

Isso instalará o Oh My Zsh em seu sistema. Depois de instalado, você pode editar o arquivo .zshrc para ativar os plugins e temas desejados.

Para ativar um plugin, adicione o nome do plugin à lista de plugins no arquivo .zshrc. Por exemplo, para ativar o plugin zsh-autosuggestions, adicione a seguinte linha ao arquivo .zshrc:
- `plugins=(zsh-autosuggestions)`

Para ativar um tema, defina a variável ZSH_THEME como o nome do tema desejado. Por exemplo, para ativar o tema agnoster, adicione a seguinte linha ao arquivo .zshrc:
- `ZSH_THEME="agnoster"`
## Conclusão
A Zsh é uma poderosa shell de linha de comando que oferece muitos recursos e personalizações em comparação com as shells padrão. Com o conhecimento básico deste manual, você pode começar a usar a Zsh de forma efetiva e personalizá-la de acordo com suas necessidades. Além disso, com plugins e temas adicionais, você pode estender ainda mais a funcionalidade da Zsh e personalizar sua aparência.
