# oop-queue-config

This is the RabbitMQ configuration for Open Interop.

## Installation

The Open Interop microservices depend on RabbitMQ. Installtion instructions can be found [here](https://www.rabbitmq.com/download.html).

Once RabbitMQ is installed, you can apply the configuration by running `sudo rabbitmqadmin import rabbit-config.json`.

## Rabbit Configuration

Most messages are be published to the `oop` exchange. Rendered temprs are published to the `oop.endpoints` exchange, which then routes messages to the `oop.endpoints.*` queues. Errors are published to `oop.errors`.

## Microservice Config

`.env.all.example` contains all available environment variables with example values.

## Contributing

We welcome help from the community, please read the [Contributing guide](https://github.com/open-interop/oop-guidelines/blob/master/CONTRIBUTING.md) and [Community guidelines](https://github.com/open-interop/oop-guidelines/blob/master/CODE_OF_CONDUCT.md).

## License

Copyright (C) 2020 The Software for Health Foundation Limited

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU Affero General Public License as
published by the Free Software Foundation, either version 3 of the
License, or (at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU Affero General Public License for more details.

You should have received a copy of the GNU Affero General Public License
along with this program.  If not, see <https://www.gnu.org/licenses/>.
