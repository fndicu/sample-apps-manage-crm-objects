# HubSpot-ruby CRM-objects sample app

### Requirements

1. Make sure you have [Python 3.8+](https://www.python.org/downloads/) installed.
2. [Configured](https://github.com/HubSpot/sample-apps-manage-crm-objects/blob/main/README.md#how-to-run-locally) .env file

### Running

1. Install dependencies

```
pip3 install -r requirements.txt
```

2. Commands

Show all commands (get help)

```
python cli.py -h
```

Get objects

```
python cli.py -m get_page -t [object_type]
```

Get an object by Id

```
python cli.py -m get_by_id -t [object_type] -i [object_id]
```

Creare new object

```
python cli.py -m create -t [object_type] -p [params]
```

Params is a json, example:

```
'{"email":"some@email.com","firstname":"Some","lastname":"One"}'
```

Delete an object by Id

```bash
python cli.py -m archive -t [objectType] -i [objectId]
```

Update an object by Id

```bash
python cli.py -m update -t [objectType] -i [objectId] -p [params]
```

Params is a json, example:

```
'{"firstname":"New"}'
```
