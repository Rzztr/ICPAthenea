# `Athenea`

Athenea, es un proyecto en ICP desarrollado por la Universidad Tecnologica de Ags. Acerca de un boton de panico que se centraliza en la seguridad del usuario dando una geolocalizacion y dando ayuda a la persona afectada, tambien ofrece servicios centralizados para la mujer, personas mayores y niñas dando asi mas informacion necesaria para su vida diaria y protegiendolos al mismo tiempo. 

"Siempre contigo, siempre segura". Athenea


Olimpo's notes: 
###NOTA DE USO DE ATHENEA RAR

Se subio en forma rar ya que ICP tiene conflictos de librerias en el uso de nombres de carpetas y de busquedas de archivos, la parte fundamental esta en el uso de un servidor propio de recepcion de datos y de interpretacion mediante la apli en el archivo correspondiente. 

METODO DE USO: 
  cd atheneaContinuo
  python3 app.py

  Abres tu navegador en http://127.0.0.1:5000 (se le pone /consultas - /login dependiendo de la pagina)

Como se planea a manera estatal el proyecto, se prueba en servidores locales y redes internas, en caso de ser testeado en produccion, se necesita apis de google y servicio de host o montar el servidor en el area....


Nota para Ricardo: 
Ewe, con ICP vamos a tardar y gastar mas para que sea compatible con lo nuestro, porque usamos ICP si no es compatible y hay mas errores que funcionalidades para hackeo etico (?)....



ICP Development:

To learn more before you start working with `Athenea`, see the following documentation available online:

- [Quick Start](https://internetcomputer.org/docs/current/developer-docs/setup/deploy-locally)
- [SDK Developer Tools](https://internetcomputer.org/docs/current/developer-docs/setup/install)
- [Motoko Programming Language Guide](https://internetcomputer.org/docs/current/motoko/main/motoko)
- [Motoko Language Quick Reference](https://internetcomputer.org/docs/current/motoko/main/language-manual)

If you want to start working on your project right away, you might want to try the following commands:

```bash
cd Athenea/
dfx help
dfx canister --help
```

## Running the project locally

If you want to test your project locally, you can use the following commands:

```bash
# Starts the replica, running in the background
dfx start --background

# Deploys your canisters to the replica and generates your candid interface
dfx deploy
```

Once the job completes, your application will be available at `http://localhost:4943?canisterId={asset_canister_id}`.

If you have made changes to your backend canister, you can generate a new candid interface with

```bash
npm run generate
```

at any time. This is recommended before starting the frontend development server, and will be run automatically any time you run `dfx deploy`.

If you are making frontend changes, you can start a development server with

```bash
npm start
```

Which will start a server at `http://localhost:8080`, proxying API requests to the replica at port 4943.

### Note on frontend environment variables

If you are hosting frontend code somewhere without using DFX, you may need to make one of the following adjustments to ensure your project does not fetch the root key in production:

- set`DFX_NETWORK` to `ic` if you are using Webpack
- use your own preferred method to replace `process.env.DFX_NETWORK` in the autogenerated declarations
  - Setting `canisters -> {asset_canister_id} -> declarations -> env_override to a string` in `dfx.json` will replace `process.env.DFX_NETWORK` with the string in the autogenerated declarations
- Write your own `createActor` constructor
# ICPAthenea
"# ICPAthenea" 

