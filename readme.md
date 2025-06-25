# 📚 Biblioteca Flutter

Um app Flutter moderno e animado para explorar livros, com suporte a favoritos, tema escuro, cache offline e animações suaves.

---

## 🚀 Instruções de Execução

1. **Clone o repositório:**

```bash
git clone <[url-do-repositorio](https://github.com/kpierroti/booklist)>
cd biblioteca_flutter
```

2. **Instale as dependências:**

```bash
flutter pub get
```

3. **Execute o app:**

```bash
flutter run
```

> **Requisitos:** Flutter SDK 3.10+ instalado e configurado

---

## 📦 Bibliotecas Utilizadas

| Pacote                      | Finalidade                       |
| --------------------------- | -------------------------------- |
| `provider`                  | Gerenciamento de estado          |
| `shared_preferences`        | Cache local (offline)            |
| `rxdart`                    | Debounce em busca reativa        |
| `flutter_lints`             | Padronização e boas práticas     |
| `flutter_animated` (nativo) | Animações integradas com Flutter |

---

## ⚙️ Decisões Técnicas

### 🧩 Arquitetura

- **Modularizada**, com separação clara entre:
  - `models/`
  - `views/`
  - `components/`
  - `providers/`
  - `services/`

### 🎨 Tema e Estilo

- Dois temas (`claro` e `escuro`) baseados em **amarelo e roxo**
- Customização centralizada em `theme.dart`

### 🧠 Estado

- `Provider` para controle de livros e favoritos
- Busca com debounce usando `rxdart`

### 💾 Offline First

- Cache persistente dos livros e favoritos com `SharedPreferences`
- Fallback automático e aviso via `SnackBar` quando sem conexão

### 🎬 Animações

- **Hero Animation** para transição entre lista e detalhe
- **AnimatedSwitcher** no botão de favoritos
- **Slide + FadeTransition** nos itens da lista
- **Skeleton Loader** para carregamento inicial

---

## 📱 Telas

- Listagem de livros
- Busca com filtro reativo
- Tela de detalhes com botão de favoritos
- Lista de favoritos

---

## ✨ Melhorias Futuras

- Integração com API real
- Lottie para carregamento ou estados vazios
- Splash screen personalizada
- Testes unitários e de widget

---

Desenvolvido com 💜 em Flutter

