ignore %r{.nfs\h+}, %r{.swp$}, %r{~$}

guard 'jade', :output => 'build', :all_on_start => true do
  watch(%r{^src/(.+\.jade$)})
end

guard :copy, :from => 'src', :to => 'build', :mkpath => true, :run_at_start => true, :verbose =>true do
	watch(%r{^src/(?!.+(\.jade)$)(.+$)})	
end
