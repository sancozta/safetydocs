## Kivy

>Neste diretório fica salvo todos os arquivos referentes a documentação especifica do kivy. 

<p style="text-align: justify;">
O Kivy é um framework para desenvolvimento de aplicativos mobile com a linguagem python. Esse framework teve seu nascimento em 2011 e possui uma comunidade forte e presente no desenvolvimento de suas soluções. Kivy é totalmente de graça. Mesmo se seu projeto estiver lucrando em cima de soluções desenvolvidas com Kivy, você não deve nada à comunidade Kivy.
</p>

<p style="text-align: justify;">
Com Kivy tudo é rápido, isso se aplica tanto à velocidade de desenvolvimento quanto à velocidade de execução dos aplicativos criados com Kivy. Para ser rápido, o Kivy foi otimizado de diversas formas. Alguns de seus módulos mais críticos foram feitos inteiramente em C, para utilizar o poder de seus compiladores.
</p>

<p style="text-align: justify;">
Uma grande característica do Kivy é a questão multiplataforma, que roda tanto em dispositivos mobile como também em desktops. Por ser escrito com python o código do nosso projeto com Kivy fica bem menor comparado a outros frameworks de mercado. O código da parte mobile do projeto pode ser encontrado em <a href="https://github.com/sancozta/safetykivy">sancozta/safetykivy</a>.
</p>

### Estrutura

#### api

Pasta que contém os arquivos referentes a comunicação com a Api.

#### home

Pasta que contém os arquivos referentes a tela principal do aplicativo.

#### imgs

Pasta que contém as imagens utilizadas pelo projeto.

#### login

Pasta que contém os arquivos referentes a tela de login do aplicativo.

#### manager.py

Arquivo para gerenciamento das telas e suas transições.

#### .gitignore

É apenas um arquivo para que no repositório git não seja versionado arquivos temporários.

#### main.py

Arquivo principal que é executado para inicialização da aplicação.

#### readme.md

Arquivo que contém os comandos necessários para executar o aplicativo localmente.

#### requirements.txt

Arquivo onde registramos todos os pacotes necessários para a execução da aplicação.

### Preparando Ambiente

<p style="text-align: justify;">
Para executar o aplicativo primeiro é necessário que o Kivy esteja instalado. Para instalar o Kivy precisamos que o Python esteja instalado na nossa máquina, com isso executando os comandos abaixo teremos o Kivy em nosso ambiente e assim estaremos prontos para executar nossa aplicação.
</p>

    python -m pip install --upgrade pip wheel setuptools
    python -m pip install docutils pygments pypiwin32 kivy.deps.sdl2 kivy.deps.glew
    python -m pip install kivy.deps.gstreamer
    python -m pip install kivy.deps.angle
    python -m pip install kivy 

### Instalando Dependências

<p style="text-align: justify;">
Após instalar o Kivy precisamos baixar todas a dependência especificas e necessárias para o nosso projeto, fazemos isso executando o comaando abaixo.
</p>

    pip install -r requirements.txt

### Executando Aplicativo

Agora para abrir o aplicativo entre na pasta do aplicativo e execute o comando abaixo.

    python main.py

Com isso o Kivy abrirá o aplicativo em uma janela do seu desktop e você poderá utilizar o aplicativo como se estivese sendo executado em um smartfone.

### Android Debug Bridge

<p style="text-align: justify;">
O Android Debug Bridge (ADB) é uma ferramenta de linha de comando versátil que permite a comunicação com uma instância de emulador ou com um dispositivo Android conectado. Ele facilita uma variedade de ações de dispositivo, como instalar e depurar aplicativos.
</p>

Como usar a ferramenta para depurar aplicativos:

	1 - Ative o modo de depuração do aparelho e conecte ao PC.
	2 - Usando o cmd (ou similar) navegar até a pasta que contém o adb.exe.
	3 - Digite: adb devices.
	4 - No dispositivo, no popup que surgir, permita o acesso.
	5 - Volte para o cmd e digite: adb logcat.

Pronto, na tela no cmd irá listar os logs de todos os aplicativos.