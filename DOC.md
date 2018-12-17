# Up and running

- watch https://www.youtube.com/watch?v=k5E2AVpwsko

- install (globally) **LTS** version of node https://nodejs.org/en/download/

- `node --version` _(min version 6.9)_

- `npm install -g @angular/cli` _(-g install globally)_

- `ng --version`

- `ng new hello-world`

- `cd hello-world` (need to be within the project you've created)

- `ng serve` _(starts a local session and a watch for changes)_

- likely http://localhost:4200

# Angular methodology

> **Modules** (groups of related Components)
>
> > **Components** (building blocks grouped by related content)
> >
> > > **Template (Markup)** (can create / define custom tags which match the Component used)
> > >
> > > > **Directives** (html attribute(s) on an element that add logic to how that element is rendered)
> > > >
> > > > - ex: <li **\*ngFor="let _item_ of _array_"**></li\>
> > >
> > > **Style**
> > >
> > > **TypeScript**
> > >
> > > **Data** (served thru a Component's class. Optionally: provided by an external service)
> >
> > **Service** (a static object of data or provided by an HTTP endpoint)

# Shortcuts

- `cd hello-world` (need to be within the project you've created)

- `ng g c component_name` (automates creation of an Angular Component. g: generate, c: component)

- `ng g s service_name` (automates creation of an Angular Service. g: generate, s: service) _\*NOTE: the service still **needs to be provided** within the main app_
  > in **src/app/app.module.ts**
  >
  > @NgModule({...**providers: [*service_name*]**...})
