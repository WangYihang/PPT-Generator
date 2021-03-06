# PPT Generator
#### Requirements
```
python-pptx
anytree
```

#### Installation
```
pip install -r requirements.txt
git clone https://github.com/c0fec0de/anytree
cd anytree
sudo python setup.py install
```

#### Usage
```
➜  PPT-Generator git:(master) python generator.py 
Usage: 
	python generator.py [INPUT] [OUTPUT]
Example: 
	python generator.py input.txt output.pptx
```

#### Example
```
➜  PPT-Generator git:(master) cat input.txt 
Slide 1
    Slide 1.1
    Slide 1.2
    Slide 1.3
    Slide 1.4
Slide 2
    Slide 2.1
        Slide 2.1.1
        Slide 2.1.2
    Slide 2.2
        Slide 2.2.1
        Slide 2.2.2
        Slide 2.2.3
        Slide 2.2.4
        Slide 2.2.5
            Slide 2.2.5.1
Slide n
➜  PPT-Generator git:(master) python generator.py input.txt output.pptx
root
├── Slide 1
│   ├── Slide 1.1
│   ├── Slide 1.2
│   ├── Slide 1.3
│   └── Slide 1.4
├── Slide 2
│   ├── Slide 2.1
│   │   ├── Slide 2.1.1
│   │   └── Slide 2.1.2
│   └── Slide 2.2
│       ├── Slide 2.2.1
│       ├── Slide 2.2.2
│       ├── Slide 2.2.3
│       ├── Slide 2.2.4
│       └── Slide 2.2.5
│           └── Slide 2.2.5.1
└── Slide n
```

![image.png](https://upload-images.jianshu.io/upload_images/2355077-2a1ecdfca171a2e7.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![image.png](https://upload-images.jianshu.io/upload_images/2355077-16fe4b49f622e2cd.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

#### Acknownledgement
Thanks for the great support of these repos:  

* https://github.com/c0fec0de/anytree
* https://github.com/scanny/python-pptx  
