# Fedora Linux

## How to differentiate between various variants of Fedora

> Through `VARIANT` and `VARIANT_ID`.

* Workstation
  
  ```
  VARIANT="Workstation Edition"
  VARIANT_ID=workstation
  ```

* Server

  ```
  VARIANT="Server Edition"
  VARIANT_ID=server
  ```

* CoreOS

  ```
  VARIANT="CoreOS"
  VARIANT_ID=coreos
  ```
  
* IoT 
  
  ```
  VARIANT="IoT Edition"
  VARIANT_ID=iot
  ```

* Cloud

  ```
  VARIANT="Cloud Edition"
  VARIANT_ID=cloud
  ```

* Silverblue
  
  ```
  VARIANT="Silverblue"
  VARIANT_ID=silverblue
  ```
* Kinoite

  ```
  VARIANT="Kinoite"
  VARIANT_ID=kinoite
  ```

* Sericea

  ```
  VARIANT="Sericea"
  VARIANT_ID=sericea
  ``` 

* Container

  ```
  VARIANT="Container Image"
  VARIANT_ID=container
  ```

## Spec file

In Fedora, the package contains `/etc/os-release` is 
[`fedora-release`](https://src.fedoraproject.org/rpms/fedora-release).

