# INFORME – Instalación y Ejecución de xv6 (RISC-V)
**Autora:** Florencia Vidal  
**Rama:** t0-FVidal 
**Curso:** Sistemas Operativos  
**Fecha:** 2025-08-29 (18:09)

## 1. Pasos seguidos para instalar xv6
1. Instalé Xcode Command Line Tools: `xcode-select --install`.
2. Instalé Homebrew y verifiqué su funcionamiento con: `brew --version`, `brew doctor`.
3. Instalé QEMU con Homebrew:  
   - `brew install qemu`  
   - Verifiqué con: `qemu-system-riscv64 --version`
4. Instalé el toolchain RISC-V (ELF):  
   - `brew tap riscv-software-src/riscv`  
   - `brew install riscv-gnu-toolchain`  
   - Verifiqué con: `riscv64-unknown-elf-gcc --version`
5. Realicé un fork del repositorio original en mi cuenta de GitHub.
6. Cloné mi fork con GitHub Desktop y creé la rama `xv6-riscv`.
7. Compilé y ejecuté xv6 desde la raíz del proyecto:  
   - `make clean`  
   - `make qemu`
8. Probé en la shell de xv6 los siguientes comandos:  
   - `ls`  
   - `echo "Hola xv6"`  
   - `cat README`
9. Salí de QEMU con el atajo **Ctrl+a**, luego **x**.
10. Creé la carpeta `evidencias/` dentro del repositorio para guardar las capturas de ejecución.
11. Tomé y guardé las capturas de pantalla mostrando la ejecución de los comandos.

## 2. Confirmación de funcionamiento correcto
- xv6 compiló y ejecutó correctamente en QEMU.  
- Los comandos `ls`, `echo "Hola xv6"` y `cat README` funcionaron mostrando la salida esperada.  
- Se adjuntan capturas en la carpeta `evidencias/` (`xv6-ejecucion-1.png`, `xv6-ejecucion-2.png`).

## 3. Notas
- **Sistema utilizado:** macOS Ventura 13.4 (MacBook Air 13”, 2018, Intel i5, 8 GB RAM).  
- **Herramientas:** Homebrew, GitHub Desktop, Terminal (zsh), Visual Studio Code.  
