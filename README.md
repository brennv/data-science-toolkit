# startup

prereqs:
- [virtualbox](https://www.virtualbox.org/wiki/Downloads)
- [vagrant](https://www.vagrantup.com/downloads.html)

then:
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

see: build/README.md

# acknowledgements

this project is would not be possible without several other open source projects:

- [virtualbox](https://www.virtualbox.org/)
- [vagrant](https://www.vagrantup.com/)
- [jupyter](http://jupyter.org/)
- [calico](https://bitbucket.org/ipre/calico)
- [many](https://github.com/datascienceinc/data-science-toolkit/blob/master/build/ansible/roles/jupyter/tasks/analysis-deps.yml) python community libraries

# similar projects

https://github.com/DataScienceToolbox/data-science-toolbox/
https://github.com/jpadilla/juicebox
