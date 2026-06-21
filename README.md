# Compiler-Creation
# ORIENTAÇÕES
## Alunos
- Amora Marinho Machado
- Enzo Dante Mícoli
- Pedro Bizzari

## Instalações
Primeiro garanta que você tenha feito o seguinte comando:
- `sudo apt install flex bison llvm nasm`
- `sudo apt install build-essential`
- em seguida extraia os arquivos para sua pasta e dentro dela rode `make` e então irá criar o compilador
- compilador se chama `valc`, então para compilar um arquivo faça: `./valc meuPrograma.val`
- então rode o programa com `./meuPrograma` (no caso esse é o executável gerado)

## exemplo de programa
```cpp
int main(){
    int x = 0;
    int a = x + 5;
    print("valor de a = {a}");
    return 0;
}
```
```cpp
int main(){
    int x = 2;
    if(x > 5){
        print("x maior que 5");
    }else{
        print("x menor que 5");
    }
    return 0;
}
```

## alguns prompts principais utilizados
- IA utilizadas, Copilot e Claude

### Prompts:
- O que preciso instalar no sudo para criar um compilador?
- - ```sh
sudo apt install flex bison llvm nasm
sudo apt install build-essential```

- como funciona o comando `make`?
- - O comando make procura um arquivo chamado Makefile no diretório atual.
- - Esse arquivo contém as regras de compilação (como transformar .l em .c, .y em .c, e depois compilar tudo com g++).
- - Ao rodar make, ele gera o executável final do compilador (normalmente chamado compiler, a.out ou o nome que você definir no Makefile).

- O que precisa para gerar o executável?
- - arquivo ast.hpp ele é o responsável por criar o executável do seu programa após compilar

- Crie um exemplo simples e completo de um compilador
- - aqui a ia criou um exemplo de compilador onde usamos para trabalhar no nosso projeto de compiladores