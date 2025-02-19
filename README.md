# Desktop-Cleaner
python notebook for cleaning different formats files into certain folders

# Instruction for running:
1. put the notebook into the folder or drive you want to clean.
2. Open the notebook on Vs code.
3. run cells from top to bottom
---
## code explanation:

- First cell imports libraries
- The second cell gets the address of the directory cleaner notebook placed.
- The third cell gets the list of files in the directory and uses it for moving files to the proper folder based on format.
---
## What if the format you are looking for is not in the third cell:

by adding another line to the if series you can create you proper folder and also put files based on the format you want for example:
---
```
elif file.endswith('format you want'):
        try:
            os.mkdir('name of folder')
            shutil.move(f'{address}/{file}',f'{address}/python files/{file}')
        except:
            shutil.move(f'{address}/{file}',f'{address}/python files/{file}')
```
---
you can also add more formats to the same folder by adding **or** to the condition of **elif** :
---
```
or file.endswith('format you want')
```
---
