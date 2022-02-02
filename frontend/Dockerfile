FROM node:10.4 as builder
#WORKDIR /
ADD . .
#COPY ./package.json ./ 
#COPY ./package-lock.json ./ 
RUN npm install
#copy ./public/ ./
RUN npm run build

#CMD tail -f /dev/null
CMD npm start run --host 0.0.0.0:3000
#FROM node:10.4 as runner
#COPY --from=builder /build/ /
#copy 
#WORKDIR /var/www
#expose 3000
#RUN npm start run --host 0.0.0.0:3000
#не понятно мне какие файлы являются необходимыми после сборки артефакта,
#поэтому не знаю что именно нужно перенести на новый образ. Ну не программист я.

