
# Reducing tailwind css to only include classes used in html:
NODE_ENV=production tailwind build src/tailwind/tailwind.css -c src/tailwind/tailwind.config.js -o atis-tailwind-default-free/assets/css/tailwind/tailwind-theme.css

# Minifying minimal tailwind css:
cleancss -O 1 --source-map --source-map-inline-sources --output atis-tailwind-default-free/assets/css/tailwind/tailwind-theme.min.css atis-tailwind-default-free/assets/css/tailwind/tailwind-theme.css
