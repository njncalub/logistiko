# BI Dashboard for Logistics

Sample project for emulating the Business Intelligence dashboards of logistics applications.

## Requirements

* Python 3.6+
* PostgreSQL 10.3+

## Dependencies

This project uses [pipenv](https://github.com/pypa/pipenv) to install Python dependencies.

## Getting Started

Create an alias for `pipenv run python` in your `~/.bash_profile`:

```
alias prp="pipenv run python"
```

Install project dependencies:

```
$ pipenv install
```

Set your environment variables in the `.env` file:

```
$ cp .env.example .env
$ vi .env
```

This file will automatically be loaded by pipenv.

## Initialize the database

```
$ pipenv run python app.py init_db
```

## Load data from existing Excel and CSV files.

```
$ pipenv run python app.py load_analysis <path to file>
$ pipenv run python app.py load_sales_order --item <path to file>
$ pipenv run python app.py load_sales_order --item_status <path to file>
$ pipenv run python app.py load_sales_order --item_status_history <path to file>
```

## Running the server and viewing the dashboard.

```
$ pipenv run python app.py run
```

## License

MIT. See [LICENSE.md](LICENSE.md) for more details.
