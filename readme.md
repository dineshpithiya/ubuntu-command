## Unix zip directory but excluded specific subdirectories (and everything within them)

Suppose folder structure like
```
a-folder-name
	-b
		-1
		-2
	-c
		-uploads
		-2
		-3
		-4
	-d
		-a
		-b
		-c
```
Suppose no need of uploads folder data

```
zip -r a-folder-name.zip a-folder-name -x a-folder-name/c/uploads/**\* a-folder-name/c/uploads/**\*
``