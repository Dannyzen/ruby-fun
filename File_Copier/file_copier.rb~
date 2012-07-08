require 'FileUtils'
require 'json'
require 'parseconfig'

#using the magical config tool get the config file and store it as a ParseConfig object
config = ParseConfig.new('config')

#File copier function. Takes a source and destination. Get's the source files' base directory, makes a new directory in the destionation, then copies the file to that folder
def copy_with_path(src, dst)
	src_folder = File.basename(File.dirname(src))
	newpath = (dst + src_folder)
	FileUtils.mkdir_p(newpath)
 	FileUtils.cp(src, newpath)
end

#this dude gets all the files you're looking for 
all_files = Dir.glob (config['source_folder'] + config['file_type'])


#for each one of the files you found, use the copy_with_path function
all_files.each {|file| copy_with_path(file, config['destination'])}


