# Configuration #

Include the gwt-touch jar file in your project, and inherit the toolkit in your application's module.xml file:
```
  <inherits name="com.googlecode.gwttouch.Touch"/>
```


We also recommend that you only compile for Safari, since both Android and iOS use the underlying webkit engine:
```
  <set-property name="user.agent" value="safari"/>
```

# Hello World #

_coming soon_