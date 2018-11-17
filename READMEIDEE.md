# project
LA STRUCTURE D'UN MODULE ZEND
Vous pouvez étendre les fonctionnalités de Omeka S en écrivant un composant supplémentaire appelé module. Zend Framework 2 fournit un cadre substantiel pour l'écriture de modules , mais Omeka S fournit une structure supplémentaire qui permet d'installer les modules, de les mettre à niveau et de les intégrer.
MyModule/
    Module.php
    config/
        module.ini
        module.config.php
    src/
        <library-directories-and-files>
    assets/
        <asset-directories-and files>/
    view/
        <module-namespace>/
            <controller-directories>/
                <action-template-files>.phtml
        common/
          mymodule-<template-files>.phtml
         
Le nom du répertoire du module ( MyModuleci-dessus) est significatif. Il doit s'agir d'un nom raisonnablement unique, concis et descriptif de votre module au format CamelCase.

Le assetrépertoire contient des actifs tels que JavaScript, CSS et des fichiers image, généralement dans leurs propres sous-répertoires.

Lorsque vous utilisez un répertoire partagé dans le viewrépertoire (comme commonci-dessus), veillez à nommer les modèles de manière à éviter les conflits de noms. Une bonne pratique consiste à préfixer les noms de modèles avec le nom de votre plugin.
Omeka S suit le même esprit et les mêmes principes d’Omeka Classic, qui consiste à utiliser un logiciel open source pour aider les institutions du patrimoine culturel à rendre leurs fonds accessibles sur le Web. Le code, cependant, est complètement différent. Ce qui suit est un guide rapide sur les différences entre les grandes lignes. Vous aurez envie de lire les sections sur les concepts clés pour plus de détails.
