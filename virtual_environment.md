1. transfer to local computer
```
echo $PATH  
PATH=/bin:/usr/bin:$PATH  
export PATH  
ssh lu_zhao@xx.xxx.xx.xxx -L 7999:localhost:7999  
```

2.download anaconda for python3.7 from website
```
wget https://repo.anaconda.com/archive/Anaconda3-2019.03-MacOSX-x86_64.pkg
```

3. install anaconda
```
bash xxxxxx.sh
```

4. source the bashrc
```
source ~/.bash
```

5.create the virtual environment and install the pip inside the virtual environment (important)
```
conda create -n <venv name> pip 
```

6. activate the virtual environment
```
conda activate <venv name> 
```

7. install ipykernel inside the venv (important)
```
pip install ipykernel
```

8. register the kernel into jupyter notebook
```
python -m ipykernel install --user --name <venv name> --display-name "<venv name>"
```

9. check whether pip in inside the virtual environment
```
which pip
```

10. install the packages inside the virtual environment
```
pip xxxxxx
```
