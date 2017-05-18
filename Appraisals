RAILS_VERSIONS = %w(
  4.0.13
  4.1.15
  4.2.8
  5.0.3
  5.1.1
)

RAILS_VERSIONS.each do |version|
  appraise "rails_#{version}" do
    gem 'rails', version
    gem 'mysql2', '~> 0.3.18' if version == '4.1.15' || version == '4.0.13'
  end
end