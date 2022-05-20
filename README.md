



## Clone app
`git clone https://myapp-repo/ app`

For example:
`git clone  https://github.com/bjfish/rails-blog-sqlite.git app`
Update `.ruby-version` file to `3.0.3`

# Build
docker build -t rbenv:test .

# Run
1. docker run -it rbenv:test bash -l -c 'source ~/.bashrc && cd /root/app && bin/rails db:migrate'

2. docker exec -it {your_container_name} bash -l -c 'source ~/.bashrc && cd /root/app && rails db:migrate' 

3. Visit http://localhost:3000/