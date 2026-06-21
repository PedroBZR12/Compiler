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