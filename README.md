flowchart TD
    subgraph FASE1[🔴 FASE 1: CRIAÇÃO DA REVISTA]
        A1[1.1 Acessar Admin do Site<br/>/index.php/index/admin]
        A2[1.2 Revistas Hospedadas → Criar Revista]
        A3[1.3 Preencher dados básicos<br/>Nome, Sigla, Descrição, Caminho]
        A4[1.4 Configurar Identidade<br/>ISSN, Contato, Foco e Escopo]
        A5[1.5 Criar Seções Editoriais<br/>Artigos Originais, Revisões, Editoriais]
        A6[1.6 Configurar Fluxo de Trabalho<br/>Avaliação duplo-cega, Prazos]
        A7[1.7 Criar Formulário de Avaliação<br/>Critérios personalizados]
        A8[1.8 Configurar Aparência<br/>Logo, Cores, CSS]
        A9[1.9 Definir Políticas de Acesso<br/>Acesso Aberto, Licença CC]
    end

    subgraph FASE2[🟠 FASE 2: CADASTRO DE USUÁRIOS]
        B1[2.1 Cadastrar Editores<br/>Gerente, Editor-Chefe, Editores de Seção]
        B2[2.2 Cadastrar Avaliadores<br/>Importar em lote ou manual]
        B3[2.3 Cadastrar Autores<br/>Individual ou em lote]
        B4[2.4 Definir Papéis e Permissões<br/>Atribuir responsabilidades]
    end

    subgraph FASE3[🟡 FASE 3: SUBMISSÃO DE ARTIGOS]
        C1[3.1 Autor acessa revista<br/>Fazer Submissão]
        C2[3.2 Passo 1: Início<br/>Idioma, Seção, Checklist]
        C3[3.3 Passo 2: Upload<br/>Arquivo anonimizado .docx/.pdf]
        C4[3.4 Passo 3: Metadados<br/>Título, Resumo, Keywords, Autores]
        C5[3.5 Passo 4: Confirmação<br/>Revisão dos dados]
        C6[3.6 Passo 5: Envio<br/>Protocolo gerado, e-mail enviado]
        
        C7[3.7 Repetir para Artigos 2, 3, 4...<br/>Múltiplos artigos e autores]
    end

    subgraph FASE4[🟢 FASE 4: TRIAGEM EDITORIAL]
        D1[4.1 Editor recebe e-mail<br/>Nova submissão recebida]
        D2[4.2 Acessar painel<br/>Minhas Submissões Designadas]
        D3[4.3 Abrir submissão<br/>Verificar arquivo e metadados]
        D4{4.4 Decisão na Triagem}
        D5[Aceitar para avaliação]
        D6[Solicitar revisões]
        D7[Rejeitar]
    end

    subgraph FASE5[🔵 FASE 5: AVALIAÇÃO POR PARES]
        E1[5.1 Editor designa avaliadores<br/>Mínimo 2, recomendado 3]
        E2[5.2 Sistema envia convites<br/>E-mail com botões Aceitar/Recusar]
        E3[5.3 Avaliador aceita<br/>Acessa sistema]
        E4[5.4 Avaliador baixa artigo<br/>Lê e analisa]
        E5[5.5 Avaliador preenche formulário<br/>Critérios pré-definidos]
        E6[5.6 Avaliador emite recomendação<br/>Aceitar/Revisões/Rejeitar]
        E7[5.7 Sistema notifica editor<br/>Parecer recebido]
        E8[5.8 Repetir para todos avaliadores<br/>Aguardar 2-3 pareceres]
    end

    subgraph FASE6[🟣 FASE 6: DECISÃO EDITORIAL]
        F1[6.1 Editor analisa pareceres<br/>Consolida feedback]
        F2{6.2 Decisão do Editor}
        F3[Aceitar]
        F4[Solicitar Revisões Obrigatórias]
        F5[Reapresentar para Avaliação]
        F6[Rejeitar]
        
        F7[6.3 Enviar e-mail ao autor<br/>Com pareceres consolidados]
    end

    subgraph FASE7[🟤 FASE 7: REVISÃO DO AUTOR]
        G1[7.1 Autor recebe e-mail<br/>Pareceres e solicitações]
        G2[7.2 Autor analisa comentários<br/>Identifica correções necessárias]
        G3[7.3 Autor corrige artigo<br/>Atende pontos obrigatórios]
        G4[7.4 Autor elabora carta-resposta<br/>Detalha cada correção]
        G5[7.5 Autor faz upload<br/>Nova versão + carta-resposta]
        G6[7.6 Autor reenvia ao sistema]
    end

    subgraph FASE8[🔴 FASE 8: EDIÇÃO DE TEXTO]
        H1[8.1 Editor designa copyeditor]
        H2[8.2 Copyeditor baixa artigo<br/>Versão aceita]
        H3[8.3 Revisão textual<br/>Gramática, ortografia, estilo]
        H4[8.4 Padronização<br/>Referências, citações, normas]
        H5[8.5 Envia ao autor para aprovação]
        H6[8.6 Autor aprova ou solicita ajustes]
        H7[8.7 Versão final aprovada]
    end

    subgraph FASE9[🟠 FASE 9: PRODUÇÃO E GALERIAS]
        I1[9.1 Editor designa diagramador]
        I2[9.2 Diagramador cria galerias<br/>PDF, HTML, XML JATS]
        I3[9.3 Upload do PDF final<br/>Formatado com normas]
        I4[9.4 Upload do HTML<br/>Versão responsiva]
        I5[9.5 Configurar DOI<br/>Registrar no CrossRef]
        I6[9.6 Verificar metadados finais<br/>Títulos, resumos, autores, ORCID]
    end

    subgraph FASE10[🟡 FASE 10: PUBLICAÇÃO]
        J1[10.1 Editor agenda na edição<br/>Seleciona volume/número]
        J2[10.2 Define paginação<br/>Ex: 1-15 ou e-location ID]
        J3[10.3 Clique em Publicar<br/>Artigo fica visível]
        J4[10.4 Sistema notifica autores<br/>Artigo publicado]
        J5[10.5 Atualiza indexadores<br/>Google Scholar, DOAJ, OAI-PMH]
        J6[10.6 Divulgação<br/>Redes sociais, newsletter]
    end

    FASE1 --> FASE2
    FASE2 --> FASE3
    FASE3 --> FASE4
    FASE4 --> D4
    D4 --> D5
    D4 --> D6
    D4 --> D7
    D5 --> FASE5
    D6 --> G1
    D7 --> Z1[❌ Processo Encerrado]
    
    FASE5 --> FASE6
    FASE6 --> F2
    F2 --> F3
    F2 --> F4
    F2 --> F5
    F2 --> F6
    
    F3 --> FASE8
    F4 --> FASE7
    F5 --> FASE5
    F6 --> Z1
    
    FASE7 --> FASE5
    FASE8 --> FASE9
    FASE9 --> FASE10
    
    FASE10 --> J3
    J3 --> K[🎉 ARTIGO PUBLICADO]
