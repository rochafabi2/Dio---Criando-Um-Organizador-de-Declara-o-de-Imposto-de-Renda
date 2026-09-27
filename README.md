# Dio--Criando-Um-Organizador-de-Declara-o-de-Imposto-de-Renda
Tarefa para conclusão de módulo do curso Santander- Excel com IA e Claude -  Criando Um Organizador de Declaração de Imposto de Renda

##  Visão Geral
Para essa tarefa, foi criada um planilha com três abas onde dados são solicitados para a facilitação do preenchimento do imposto de renda.


## ✨ Funcionalidades

- **Cadastro Completo:** Centralização de CPF, Título de Eleitor, endereço formatado e questionário de controle fiscal.
- **Soma Automatizada de Saldos:** Totalizador dinâmico dos saldos informados por instituição bancária.
- **Rastreabilidade de Comprovantes:** Mapeamento nominal de arquivos PDF para cada informe bancário.
- **Validação com Base Oficial:** Lista com 50 bancos e fintechs operantes no Brasil indexados por código de compensação.
- **Registro Cronológico de Entradas:** Controle mês a mês de holerites, pró-labore e receitas líquidas/brutas.

---

## 📂 Estrutura do Repositório

```text
├── .gitignore
├── LICENSE
├── README.md
└── Criando Um Organizador de Declaração de Imposto de Renda.xlsx
    ├── 1. TITULAR
    ├── 2. INFORMES
    ├── 3. NOTAS
    └── Tabelas
🔍 Detalhamento das Abas1. TITULAR (Dados Cadastrais e Perfil Fiscal)Estrutura os dados exigidos nas telas iniciais do programa da Receita Federal (PGD IRPF):CampoFinalidadeExemplo / TipoNOMENome civil completo do contribuinteLugolina da SilvaCPFCadastro de Pessoas Físicas122158447621225NASCIMENTOData de nascimento para cálculo etário08/08/1994TÍTULO DE ELEITORIdentificador eleitoral obrigatório785411254221CÔNJUGENome ou identificação conjugalTexto ou Em brancoLOGRADOUROEndereço completo, abreviado e CEPAv. Paulista, 785 / 00000-000CONTATOTelefone fixo, celular e e-mail11 98765-5423 / teste@gmail.comCHECKLISTPerguntas de controle declaratórioSim ou NãoPerguntas de Controle Fiscal inclusas:Houve alterações da entrega anterior?Dependente cônjuge?Residente do exterior?2. INFORMES (Rendimentos e Saldos Bancários)Consolidação dos informes de rendimento fornecidos pelas instituições financeiras em 31 de dezembro:Fórmula de Consolidação (C8):Excel=SUM(E12,E17,E22)
Blocos Cadastrados (1º Banco, 2º Banco, 3º Banco...):BANCO: Selecionado a partir da base padronizada (ex.: 77 - Banco Inter, 735 - Banco Neon, 72 - Banco Rural Mais).VALOR ATUAL: Saldo em conta, aplicações financeiras ou rendimentos tributáveis informados.ANEXO 🖇️: Nome do arquivo PDF comprobatório vinculado (ex.: anexo.pdf, anexobanco2.pdf).3. NOTAS (Extrato Mensal e Holerites)Tabela para auditoria cronológica das entradas de receita auferidas ao longo do ano-calendário:DATACATEGORIAVALOR (R$)2026-09-01HOLERITE25.000,002026-10-02HOLERITE32.000,004. Tabelas (Base de Dados Auxiliar)Relação com 50 instituições bancárias contendo o código COMPE e razão social para alimentação de validação de dados nas demais abas:1 - Banco do Brasil3 - Banco da Amazônia4 - Banco do Nordeste do Brasil24 - Banco de Pernambuco29 - Banco do Estado do Rio de Janeiro33 - Banco Santander37 - Banco do Estado do Pará41 - Banco do Estado do Rio Grande do Sul44 - Banco BVA62 - Hipercard Banco Múltiplo65 - Banco Lemon66 - Banco Morgan Stanley72 - Banco Rural Mais74 - Banco J. Safra77 - Banco Inter79 - Banco JBS82 - Banco Topázio102 - XP Investimentos CCTVM S.A.104 - Caixa Econômica Federal119 - Banco Western Union do Brasil184 - Banco Itaú BBA S.A.197 - Stone Pagamentos208 - Banco BTG Pactual212 - Banco Original218 - Banco Bonsucesso229 - Banco Cruzeiro do Sul237 - Banco Bradesco241 - Banco Clássico250 - Banco de Crédito e Varejo (BCV)260 - Nubank290 - PagBank336 - C6 Bank341 - Itaú Unibanco376 - Banco JPMorgan S.A.380 - PicPay422 - Banco Safra464 - Banco Sumitomo Mitsui Brasileiro477 - Citibank600 - Banco Luso Brasileiro604 - Banco Industrial do Brasil610 - Banco VR634 - Banco Triângulo654 - Banco AJ Renner655 - Banco Votorantim707 - Banco Daycoval734 - Banco Gerdau735 - Banco Neon746 - Banco Modal748 - Banco Cooperativo Sicredi S.A.749 - Banco Simples🚀 Como UtilizarClonar o Repositório:Bashgit clone [https://github.com/](https://github.com/)<seu-usuario>/organizador-irpf.git
cd organizador-irpf
Abrir a Planilha:Execute o arquivo no Microsoft Excel, Google Planilhas ou LibreOffice Calc.Sequência de Preenchimento:Acesse a aba TITULAR e informe os dados cadastrais básicos.Acesse a aba INFORMES, selecione os bancos utilizados, informe os saldos em 31/12 e nomeie os arquivos PDF correspondentes salvos em sua pasta local.Acesse a aba NOTAS e liste as receitas auferidas mensalmente com data e categoria.Envio / Importação:Use o consolidado para preencher a declaração no PGD IRPF ou compartilhe o arquivo e a pasta de comprovantes com sua assessoria contábil.🔒 Segurança e Privacidade (LGPD)[!WARNING]Proteção de Dados Sensíveis: Planilhas preenchidas contêm números de CPF, dados bancários e patrimoniais cobertos pela LGPD (Lei Geral de Proteção de Dados - Lei nº 13.709/2018).Para evitar vazamento acidental em repositórios públicos:Mantenha no Git apenas planilhas com dados fictícios (templates).Configure o arquivo .gitignore na raiz do projeto:Snippet de código# Planilhas preenchidas
*.private.xlsx
*dados_reais*.xlsx

# Comprovantes em PDF
*.pdf
comprovantes/
anexos/
