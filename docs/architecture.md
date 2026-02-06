## Product Choice

YandexGo
<https://taxi.yandex.ru/ru_ru/>
it is an app for ordering taxis, food, groceries, merchandise, parcel delivery, car rentals, and viewing transportation schedules

## Main components

1) ![YandexGo Component Diagram](./diagrams/out/yandex-go/architecture-component/Component%20Diagram.svg)
2) ![YandexGo Component Diagram code](./diagrams/src/yandex-go/architecture-component.puml)
3) Selected components:
    Mobile App, pricing service, payment service, maps & routing service, notification sevice
4) Mobile App- source from where  user can access to service (and order taxi for example).
Pricing service - service that counts all condition and calculates price of drive.
payment service - service that makes bank operations
maps & routing service - service that makes routes for taxi drives
notification service - service that send notificatinons to the user

## Data flow

1) ![YandexGo Sequence Diagram](./diagrams/out/yandex-go/architecture-sequence/Sequence%20Diagram.svg)
2) ![YandexGo Sequence Diagram code](./diagrams/src/yandex-go/architecture-sequence.puml)
3) App inicialization
4) connects client size to the services with API and transfer tokens
5) talks to Pre ride and ride comletion

## Deployment

1) ![YandexGo Deployment Diagram](./diagrams/out/yandex-go/architecture-deployment/Deployment%20Diagram.svg)
2) ![andexGo Deployment Diagram code](./diagrams/src/yandex-go/architecture-deployment.puml)
3) user and web brauser in phyysical, then in cloud services there is Load balancer , aplication tree ect

## Assumptions

1) I assyme Yandex go uses other yandex sservices for payment transer for example
2) I assyme Yandex go make routes including information about traffic

## Open questions

1)What is dispatch service

2)What is Kefka
