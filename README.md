# SD-RMIJava

Atividade: Java RMI - Chamada de Métodos Remotos  
Disciplina: Sistemas Distribuídos - IFPR

## Objetivo
Demonstrar comunicação cliente-servidor usando Java RMI (Remote Method Invocation).

## Passo a passo de execução (testado no Codespace)

```bash
# 1. Compilar tudo
javac *.java

# 2. Gerar o stub (obrigatório no RMI clássico)
rmic HelloServer

# 3. Iniciar o registro RMI em background
rmiregistry &

# 4. Iniciar o servidor (em uma aba)
java HelloServer

# 5. Em outra aba, executar o cliente
java HelloCliente localhost
