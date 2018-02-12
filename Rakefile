require 'yaml'

#Load in the configuration file
config=YAML.load_file("_config.yml")

task :upload do
	puts "Rsync pushing to production"
	system("rsync -avP --delete . #{config['server_username']}@#{config['server_name']}:#{config['server_dir']}")
end

