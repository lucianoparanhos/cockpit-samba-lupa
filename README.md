cockpit-samba-lupa

Um módulo personalizado do Cockpit para monitorar e gerenciar compartilhamentos Samba de forma simples, visual e integrada. Desenvolvido por lupa, com foco em servidores pessoais, NAS minimalistas e sistemas baseados em Linux com suporte a Btrfs.

 

🚀 Recursos

Exibe status do Samba (smbstatus)

Mostra o conteúdo do arquivo de configuração /etc/samba/smb.conf

Lista conexões SMB ativas em tempo real

Pensado para expansão futura: edição remota, reinício de serviços, integração com Snapper/Btrfs

🔧 Tecnologias

Cockpit Web Framework

HTML + JavaScript + cockpit.spawn

Docker + Debian para ambiente de desenvolvimento isolado

📂 Estrutura do projeto

cockpit-samba-lupa/
├── docker/                 # Ambiente de desenvolvimento
│   ├── Dockerfile
│   └── docker-compose.yml
├── samba-panel/           # Módulo Cockpit real
│   ├── manifest.json
│   ├── index.html
│   ├── index.js
│   └── style.css
├── LICENSE
└── README.md

🔄 Executando localmente (modo desenvolvimento)

Requisitos:

Docker

Docker Compose

git clone https://github.com/seu-usuario/cockpit-samba-lupa.git
cd cockpit-samba-lupa/docker
docker-compose up --build

Acesse https://localhost:9090 com:

Usuário: dev

Senha: definida via passwd dev dentro do container

🌍 Modo de uso (após instalado)

No painel Cockpit, você verá uma nova entrada lateral chamada "Samba". Nela:

Visualize conexões SMB ativas

Veja os compartilhamentos atuais

Acompanhe logs do Samba

(em breve) Edite o smb.conf e reinicie serviços

🎓 Para que serve?

Ideal para:

Quem usa Samba para compartilhar arquivos na LAN

Usuários de RPi, Arch, Debian ou Ubuntu

Quem quer uma interface gráfica leve para acompanhar o Samba

Pequenos servidores caseiros com Cockpit instalado

🏆 Licença

Este projeto está licenciado sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.

✨ Contribuindo

Pull Requests são bem-vindos! Planejo adicionar suporte a:

Edição do smb.conf

Criação de novos compartilhamentos

Integração com Snapper e snapshots Btrfs

Logs e diagnóstico

Abra uma issue com sugestões ou envie melhorias diretamente.

Desenvolvido com carinho por lupa.
Leve, prático e direto ao ponto.

