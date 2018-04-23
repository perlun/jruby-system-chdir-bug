def run_command(command_line)
  result = system(command_line)

  raise 'Command execution failed' if result.nil?
end

desc 'A wonderful task'
task :foo do
  Dir.chdir 'bar' do
    run_command 'BAZ=zot rake -T'
  end
end
