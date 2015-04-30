# startup

prereqs:
- virtualbox
- vagrant

```
git clone https://github.com/datascienceinc/data-science-toolkit.git
cd data-science-toolkit
vagrant up
open datascience.dev:8888
```

# shutdown

```
cd data-science-toolkit
vagrant suspend
```

# development

prereqs:
- ansible

```
cd cd data-science-toolkit/build
vagrant up
```

### packaging

```
vagrant package
```
