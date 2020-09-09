# PHP Proxy Server

Às vezes, precisamos criar um servidor proxy porque somos limitados por algo que nos impede de acessar o endereço de um site diretamente de uma máquina. Este servidor proxy encaminhará todas as solicitações recebidas para o servidor de destino.

Por exemplo: O servidor da web para o qual você está indo usa a porta 94 enquanto seu aplicativo usa hospedagem compartilhada e não pode acessar a porta 94 usando cURL devido às configurações feitas pelo provedor de hospedagem.

Você precisa de um servidor proxy para permitir o acesso de seu aplicativo à porta 94 através da porta 80.

Tudo o que você precisa fazer é criar um servidor proxy que garanta acesso à porta 94. Este servidor proxy receberá uma solicitação de seu aplicativo e, em seguida, encaminhará a solicitação para a porta 94.

Você precisa permitir a substituição do diretório raiz do documento em `httpd.conf`
