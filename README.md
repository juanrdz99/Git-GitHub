# Respuestas al ejercicio de Git

## 1. ¿Qué comando utilizaste en el paso 11? ¿Por qué?
```bash
git reset --hard HEAD~1
```
Deshizo el último commit, eliminando los cambios del working copy.

## 2. ¿Qué comando utilizaste en el paso 12? ¿Por qué?
```bash
git reflog
git reset --hard caa5f89
```
Revisé el historial de cambios y restauré el commit eliminado.

## 3. ¿El merge del paso 13 causó conflicto? ¿Por qué?
No, `styled` absorbió `main` sin conflictos.

## 4. ¿El merge del paso 19 causó conflicto? ¿Por qué?
Sí, `styled` y `htmlify` modificaron el mismo archivo de manera diferente.

## 5. ¿El merge del paso 21 causó conflicto? ¿Por qué?
No, `styled` ya contenía los cambios de `htmlify`.

## 6. ¿Qué comando utilizaste en el paso 25?
```bash
git log --graph --oneline --all
```
Mostró el historial de commits de manera visual.

## 7. ¿El merge del paso 26 pudo ser fast-forward? ¿Por qué?
No, porque se usó `--no-ff` para mantener un historial más claro.

## 8. ¿Qué comando utilizaste en el paso 27?
```bash
git reset --soft HEAD~1
```
Deshizo el merge sin perder cambios.

## 9. ¿Qué comando utilizaste en el paso 28?
```bash
git reset --hard
```
Descartó los cambios del working copy.

## 10. ¿Qué comando utilizaste en el paso 29?
```bash
git branch -d title
```
Eliminó la rama `title`.

## 11. ¿Qué comando utilizaste en el paso 30?
```bash
git merge --no-ff title
```
Rehizo el merge que se había deshecho.

## 12. ¿Qué comando usaste en el paso 32?
```bash
git checkout 8f3198cf
```
Volvió al commit inicial.

## 13. ¿Qué comando usaste en el paso 33?
```bash
git checkout main
```
Regresó al estado final del repositorio.
