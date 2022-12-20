<h1 align="center">
⛰️ Zenith Inova - Padrão de File Structure
</h1>

<h1 align="center">
  <img src="ZenithLogo.png" width="400px" height="400px">
</h1>

<h1 align="center">
🗂️ Next.js Default Folders
</h1>

A estrutura padrão de pastas do Next.js são as seguintes:
- pages - onde é aplicado o [File-system Routing](https://nextjs.org/docs/routing/introduction)
    - api - dentro de pages vai ter uma pasta chamada api, nela é onde arquivos vão rodar na aplicação node que existe dentro do Next.js. [Leia mais aqui](https://nextjs.org/docs/api-routes/introduction).

- public - vai conter os arquivos que serão públicos, será possível acessar-los pela url da aplicação. Ex.: www.aplication.com/{nome_do_arquivo}
- styles - os arquivos aqui são para configurações de estilo global(que será aplicado em toda a aplicação), geralmente são resets de css e configuração de temas. 

<h1 align="center">
📝 Padrões adotados
</h1>
Foi adotado as seguintes pastas:

- @types - onde vai ser definido tipos globais para o typescript.

- components - onde será aplicado o padrão Atomic Design.

- services - pasta onde conterá todos os serviços, microsserviços, conexão a API's, entre outros...


<h1 align="center">
⚛️ Atomic Design
</h1>

Dentro da pasta components será aplicado o padrão Atomic Design que consiste em dividir os componentes em: 
- Atoms - são blocos de construção básicos da matéria que formam a interface.
- Moléculas - grupos simples de elementos da interface do usuário que funcionam juntos como uma unidade. Vários átomos juntos.
- Organismos - conjuntos de moléculas que funcionam juntas como uma unidade. Uma molécula com outra molécula (ou mais), formam um organismo.
- Templates - saindo um pouco dos termos da química, os templates são objetos no nível de página, onde colocamos componentes em um layout formando a estrutura de página.

</br></br>
<div align="center">
<img src="atomic-design.gif" width="400px">
</div>
</br></br>

Dentro de cada pasta deve conter os seguintes arquivos: 

- [nome-do-componente].styled.ts - onde vai conter a estilização do componente

- [nome-do-componente].ts - o componente em si.

- types.ts - os tipos usados nesse componente.

