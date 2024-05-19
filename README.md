version: '3.7'

services:
  db:
    image: postgres:13-alpine
    restart: always
    environment:
      POSTGRES_DB: app
      POSTGRES_USER: app
      POSTGRES_PASSWORD: 9mREsvXDs9Gk89E
    volumes:
      - ./DZ_7:/var/lib/postgresql/data
    ports:
      - '5432:5432'

volumes:
  my-postgres-data:
