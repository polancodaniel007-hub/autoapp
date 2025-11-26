# 1. Inicializa el repositorio
git init

# 2. Crea un archivo .gitignore para excluir archivos innecesarios
echo "__pycache__/
*.pyc
*.pyo
*.pyd
.Python
venv/
env/
.env
*.log
update_temp/
update_temp.zip" > .gitignore

# 3. Crea el archivo version.txt
echo "1.0.0" > version.txt

# 4. Añade todos los archivos
git add .

# 5. Haz el primer commit
git commit -m "Versión inicial 1.0.0"

# 6. Conecta con tu repositorio de GitHub
# Reemplaza TU-USUARIO y TU-REPOSITORIO con tus datos
git remote add origin https://github.com/TU-USUARIO/TU-REPOSITORIO.git

# 7. Sube los archivos
git branch -M main
git push -u origin main
