## To deploy this project, follow this steps: <br>
1. Edit `setup.env` file with your specific cinfiguration <br>

``` -d
nano setup.env
```

2. Copy `setup.env` file to `.env` file <br>
``` -d
cp setup.env .env
```
3. Create this directories <br>
``` bash
mkdir -p ./logs/scheduler
mkdir -p ./dags
mkdir -p ./config
mkdir -p ./plugins
```
4. Setup permissions for created directories <br>
``` bash
chown -R 50000:0 ./logs
chown -R 50000:0 ./dags
chown -R 50000:0 ./config
chown -R 50000:0 ./plugins

chmod -R 775 ./logs
chmod -R 775 ./dags
chmod -R 775 ./config
chmod -R 775 ./plugins
```

5. Run docker containers <br>
``` bash
docker compose up -d
```

# Done!