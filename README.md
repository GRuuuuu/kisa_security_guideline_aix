kisa_security_guideline_aix
=========

This is Ansible Project for checking vulnerabilities in AIX server based on [KISA(Korea Internet & Security Agency Guideline)](https://www.kisa.or.kr/public/laws/laws3_View.jsp?cPage=6&mode=view&p_No=259&b_No=259&d_No=106&ST=T&SV=).  

>**WARNING!**   
>This project is only for study. and The guidelines on which this project is based were published in 2017. So please consider that there are some parts that are not correct now.

Features
-----------
1. Managing Account - `account.yml`
2. Managing File & Directory - `file_directory.yaml`
3. Managing Services - `svc_manage.yml`
4. Managing Patch & Log - `patch_n_log.yml`  

Role Variables
--------------

Global Variables are in `defaults/main.yml`  

~~~
  var_isDebug: "True"
  apche_home_dir: ""
~~~
`var_isDebug` : Set `True` if you want to print debug for each task.  
`apache_home_dir` : Set PATH if apache server runs on your target server   


Example Playbook
----------------

~~~
    - hosts: servers
      roles:
         - kisa_security_gideline_aix
~~~


Author Information
------------------
<img width="100" height="100" src="https://raw.githubusercontent.com/GRuuuuu/sawtooth-starter/master/sawtooth/%2303%20transaction%20processor%20tutorial/img/p.png"/>   

Blog : [호롤리한 하루](https://gruuuuu.github.io/)
