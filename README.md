# typescript01
Com NodeJs instalado:
npm install typescript@4.2.2 --save-dev

Configurando o COMPILADOR TYPESCRIPT
Criar um arquivo tsconfing.json:

{
    "compilerOptions":{
        "outDir": "dist/js", (pasta destino da conversão dos arquivos TS para JS = pasta dist>js)
        "target":"ES6", (converter os arquivos TS em ECMASCRIPT 6)
        "noEmitOnError": true, (não gerará arquivo js com erro)
        "strictNullChecks": true, (precisa especificar se as propriedades podem receber valor nulo)
        "experimentalDecorators": true (ativar decorators)
    },
    "include":["app/**/*"] (pasta de origem da conversão)
}



**adicionar no arquivo package.json
"compile": "tsc" (transforma arquivos ts em js | compilar: npm run compile)
"watch": "tsc -w" (monitorar os arquivos das pastas que foram inseridos no *include* e atualizar automaticamente | npm run watch)
command: npm run start (executa os comandos npm run watch e npm run compile)
