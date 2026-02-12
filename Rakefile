require 'html-proofer'

task :test do
  sh "bundle exec jekyll build"

  options = {
    assume_extension: true,
    check_html: true,
    check_img_http: true,
    enforce_https: false,  # GitHub Pages handles this
    allow_hash_href: true,
    disable_external: true,  # Disabled to avoid libcurl dependency on Windows
    ignore_urls: [
      /formspree.io/,  # Formspree endpoints return 403 for HEAD requests
      /cdnjs.cloudflare.com/  # CDN URLs might fail in tests
    ],
    ignore_status_codes: [0, 403, 999],
    typhoeus: {
      connecttimeout: 10,
      timeout: 30
    }
  }

  HTMLProofer.check_directory("./_site", options).run
end

task default: [:test]
