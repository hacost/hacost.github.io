---
layout: post
title:  "Utilizando Git / Using Git"
date:   2015-07-24 13:05:12
categories: git
---

#### **Configurar Git / Set up Git Configuration**
{% highlight powershell %}
~$ git config --global user.email "you@yourdomain.com"
~$ git config --global user.name "Your Name"
~$ git config --global core.editor "vi"
~$ git config --global color.ui true
{% endhighlight %}

Ver la configuración de Git / See Git configuration.
{% highlight powershell %}
~$ git config --list
{% endhighlight %}

#### **Inicializar un repositorio local / Initialise a local repository**
{% highlight powershell %}
~$ cd your_awesome_proyect
~$ git init
{% endhighlight %}

Agregar archivos al repositorio / Add files to the repository
{% highlight powershell %}
~$ git add file_name
#  o punto (.) para agregar todos los archivos / or dot (.) to add all files
~$ git add .
{% endhighlight %}

Confirmar el cambio a git / commit the change to git
{% highlight powershell %}
~$ git commit -m "Message goes here"
{% endhighlight %}

Ver los cambios confirmados / see the commits
{% highlight powershell %}
~$ git log
{% endhighlight %}

<br />
Git tiene 3 niveles de arquitectura / Git has a 3 Tier Architecture:
<br />
<br />
 ![git architecture](/assets/git_architecture.png)

<br /><br />

#### **Comandos básicos / Basic Commands**


<br /><br />
happy code..!
