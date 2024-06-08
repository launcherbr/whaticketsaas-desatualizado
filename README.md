# WhaTicket Versão Saas com Módulo Kanban e Modo Noturno</br>
Está é uma versão modificada pela licencas.digital da Launcher & Co.</br>
Desde 23/11/2023 este se tornou um diretório aberto, para uso livre.

Liberamos uma nova versão, confira nossos outros repositórios.

</br>Caso queira fazer uma contribuição, serei muito grato.</br>
Chave Pix, aleatória, efd3110c-e572-42b5-a6cb-5984a8811ad2.</br>

Funcionando com a última versão do Baileys 6.7.4 - Maio de 2024</br>

Apesar de ter os botões de conexões de insta e messenger, não obtivemos sucesso na conexão devida a defasagem da versão da API,
</br>contribuições para essa corrigir essa funcionalidade são bem-vindas.</br>

Notas Rápidas: </br>
Requer servidor Ubuntu 20.04 LTS com ao menos 4vcore e 8gb de ram.</br>
Recomendamos Peramix, Contabo e Hetzner. </br>
Não recomendamos Hostinger, Hostgator e Locaweb.</br>

Sugerimos a VPS Standard, a seguir:

```
https://control.peramix.com/?affid=14
```

Utilize este instalador:

```
https://github.com/launcherbr/instalador.git
```

Siga o arquivo de intruções deste repositório para instalação e fix da biblioteca e do nginx.
Confira no pdf aqui como gerar um webhook de retorno de pagamento do Efi.

Bugs Relatados:</br>
O sistema configurado 100% não tem apresentados bugs. 
</br>Exceção a instalações onde a uma discrepâncias de latência entre a instalação e os servidor de whatsapp, </br>então não funciona em localhost ou servidor local, com ping muito baixo.

Personalizações:</br>

** Alterar Cor Primária: (#007aff)</br>
```
/frontend/src/config.json</br>
/frontend/src/App.js</br>
/frontend/src/layout/index.js</br>
/frontend\src\pages\Chat\ChatMessages.js
```

** Cores do Chat Interno:</br>
```
frontend\src\pages\Chat\ChatList.js</br>
```

** Cores da Lista de Tarefas</br>
```
/frontend/src/pages/ToDoList/index.js
```

** Popover de Anúncios / Chat Interno </br>
```
/frontend/src/components/AnnouncementsPopover/index.js</br>
/frontend/src/pages/Chat/ChatPopover.js
```

** Logo e LogoLogin:</br>
```
/frontend/src/assets
```

** Icone e Favicon:</br>
```
/frontend/public
```

** Comando para rebuild, caminho absoluto /home/deploy/"nome"/</br>
Sempre que fizer alguma alteração nos arquivos é necessário rebuildar a aplicação.
  
```
cd /frontend
npm run build
```

URL WEBHOOK META:

```bash
https://api.seudominio.com.br/webhook/fb
```
