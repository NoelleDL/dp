all: hiring-process job-adverts

hiring-process:
	relaxed hiring-process.pug output/backend-engineer-hiring-process.pdf --build-once --locals '{"title":"Backend Engineer", "role": "backend-engineer"}'

job-adverts: backend-engineer-job-advert frontend-engineer-job-advert

backend-engineer-job-advert:
	relaxed job-advert.pug output/backend-engineer-job-advert.pdf --build-once --locals '{"title":"Backend Engineer", "role": "backend-engineer"}'

frontend-engineer-job-advert:
	relaxed job-advert.pug output/frontend-engineer-job-advert.pdf --build-once --locals '{"title":"Frontend Engineer", "role": "frontend-engineer"}'

.PHONY: all hiring-process job-adverts backend-engineer-job-advert frontend-engineer-job-advert