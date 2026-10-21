# 05 - MVVM · Filmes Favoritos

App Android (Kotlin + XML) para visualizar e editar filmes favoritos (nome, nota e foto).

- **View Binding**: `ActivityMainBinding`, `ItemMovieBinding`, `DialogEditMovieBinding`
- **Coil 3**: carrega as fotos (URL da internet ou imagem da galeria)
- **MVVM**:
  - `model/Movie.kt` → dados
  - `repository/MovieRepository.kt` → fonte dos dados (em memória)
  - `viewmodel/MovieViewModel.kt` → lógica (validar, adicionar, editar, excluir, desfazer) exposta via LiveData
  - `ui/MainActivity.kt` + `ui/MovieAdapter.kt` → View (só observa e repassa ações)

## Como usar
- Toque num filme para editar; botão **Adicionar** para criar.
- Lixeira exclui (com **Desfazer** na Snackbar).

## Abrir
Android Studio → *File > Open* → selecione a pasta `FilmesFavoritos` → aguarde o Gradle Sync.
