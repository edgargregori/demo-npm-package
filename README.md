# demo-npm-package

# pasos publicr un paquete en npm.

$ npm init 

    <introducir los dtos correctos, vinculados a github> 

	<Guardar los cambios en github>

$ npm publish --access=public

$ npm info


# Etiquetas
	<realizar los cambios, y package.json.>
	$ git add .
	$ git commit -m "1.1.5"
	$ git tag 1.1.5
	$ git push -u origin master
	$ git push --tags
	$ npm version patch

# Beta- La version beta no se acutaliza en la nube npm.

	realizar los cambios, y package.json.
	$ git add .
	$ git commit -m "1.1.0-beta.1"
	$ git tag 1.1.0-beta.1
	$ git push -u origin master
	$ git push --tags
	$ npm publish --tag beta

# Borrando un tag(es como una rama pero o se modifica nunca-jamas.)
	$ git tag -l # ver tags.
	$ git tag -d 1.1.0-beta.1 # borrar un tag.
	$ git push origin :refs/tags/1.1.0-beta.1 # borrar el tag de github remoto.
	$ git tag -a 1.1.0-beta.1 -m "version 1.1.0-beta.1" # adicionando un tag local.
	$ git push origin 1.1.0-beta.1 # colocando el tag en github remoto.



