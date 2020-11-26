build:
	docker build --force-rm $(options) -t mywebsite:latest .

build-prod:
	$(MAKE) build options="--target production"

compose-start:
	docker-compose up --remove-orphans $(options)

compose-stop:
	docker-compose down --remove-orpahns $(options)

compose-manage-py:
	docker-compose run --rm $(options) website python manage.py $(cmd)