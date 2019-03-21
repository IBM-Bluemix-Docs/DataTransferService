---

copyright:
  years: 2017, 2019
lastupdated: "2019-03-21"

---


# Conectando-se ao dispositivo DTS no Windows com o Inicializador de software iSCSI
{: #mountingDTSWindows}

Para interagir com uma LUN iSCSI no Windows, os usuários devem se conectar ao armazenamento usando o inicializador de software
iSCSI, uma ferramenta iSCSI proprietária da Microsoft. Para os usuários do Windows Server 2008, do Windows Vista ou de versões mais
novas, o inicializador de software iSCSI é integrado ao sistema operacional. Os usuários do Windows Server 2003, do Windows XP e do
Windows 2000 devem fazer download do inicializador antes de iniciarem esse procedimento.

## Conectando-se a uma LUN iSCSI

1. No {{site.data.keyword.slportal}}, recupere o **Nome do usuário, senha e endereço de armazenamento do iSCSI** para o dispositivo de armazenamento que você deseja conectar.
2. Inicie o Inicializador iSCSI.
3. Clique em **Descoberta**.
4. Na seção **Portais de destino**, clique em **Incluir**.
5. No campo **Endereço IP ou nome do DNS**, insira o **Endereço IP do iSCSI**.
6. Clique em **Avançado**.
7. Atualize as informações de logon de iSCSI.
   - Marque a caixa de seleção **Informações de logon do CHAP** para permitir o logon do CHAP.
   - Insira o nome do usuário do iSCSI no campo **Nome do usuário**.
   - Digite a senha do iSCSI no campo **Segredo de destino**.
   - Clique em **OK** duas vezes.
8. Clique em **Destinos**
9. Selecione o iSCSI recém-incluído na lista **Destinos**.
10. Clique em **Efetuar logon**. A janela **Efetuar logon no destino** aparece.
11. Selecione **Restaurar automaticamente essa conexão na reinicialização do sistema** para
configurar a conexão para persistir entre as reinicializações.
12. Clique em **Avançado**.
13. Atualize as informações de logon de iSCSI.
    - Marque a caixa de seleção **Informações de logon do CHAP** para permitir o logon do CHAP.
    - Insira o nome do usuário do iSCSI no campo **Nome do usuário**.
    - Digite a senha do iSCSI no campo **Segredo de destino**.
    - Clique em **OK** duas vezes.
14. Verifique se o novo destino iscsi é exibido como Conectado na guia Destinos.
    - Se o seu destino iSCSI for exibido como **Conectado**, clique em **OK**. Seu LUN iSCSI está agora conectado
    - Se o seu destino iSCSI não for exibido como **Conectado**, repita todas as etapas anteriores para reconfigurar a conexão.
