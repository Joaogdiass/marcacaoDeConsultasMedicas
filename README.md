# 🌺 Medical Appointment App - Lousa Interativa

```
📃 VISÃO GERAL
--------------------------------------------
Aplicativo para agendamento de consultas médicas:

    ✅ Escolha a Data
    ✅ Escolha o Horário
    ✅ Escolha o Médico Disponível
    ✅ Agenda com Validação de 1 ano futuro

Objetivo: Agilizar e facilitar o agendamento de consultas!
```

```
🏠 ESTRUTURA DO PROJETO
--------------------------------------------
src/
 ├── components/  → Header, DoctorList, TimeSlotList
 ├── contexts/    → AuthContext
 ├── screens/     → CreateAppointmentScreen
 ├── styles/      → theme.ts (tema de cores)
 ├── types/       → navigation.ts (tipagens)
 └── utils/       → validação de datas
```

```
🛠️ FUNCIONALIDADES
--------------------------------------------
✅ Autenticação de usuário (Context API)
✅ Validação de data futura (limite de 12 meses)
✅ Seleção de horários disponíveis
✅ Seleção de médicos
✅ Armazenamento local com AsyncStorage
✅ Validação dinâmica do formato de data DD/MM/AAAA
```

```
🔍 LÓGICA PRINCIPAL
--------------------------------------------
→ isValidFutureDate(date)
   - Confere se a data é futura e está dentro de 1 ano

→ formatDate(text)
   - Formata o texto automaticamente como DD/MM/AAAA

→ handleCreateAppointment()
   - Cria e salva a consulta localmente
```

```
🚀 COMO RODAR O PROJETO
--------------------------------------------
1. Clone o repositório:
  https://github.com/Joaogdiass/marcacaoDeConsultasMedicas.git

2. Instale as dependências:
   npm install

3. Rode no emulador ou celular:
   npx react-native run-android
   # ou
   npx react-native run-ios
```

```
🛂 DEPENDÊNCIAS PRINCIPAIS
--------------------------------------------
react-native-elements
styled-components
@react-native-async-storage/async-storage
@react-navigation/native + stacks
```

```
📌 OBSERVAÇÕES
--------------------------------------------
- Datas obrigatoriamente no formato DD/MM/AAAA
- Impede agendamentos no passado
- Impede agendamentos mais de 12 meses à frente
- Sem backend: armazenamento local
```

```
👨‍💼 AUTOR
--------------------------------------------
Nome: João Gabriel Dias de Mello do Nascimento
RM: 99092
```

