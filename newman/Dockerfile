FROM postman/newman:5

WORKDIR /etc/newman

COPY postman_collection.json .

# Install the htmlextra reporter
RUN npm install -g newman-reporter-htmlextra

# Run collection and export HTML report
CMD ["run", "postman_collection.json", "--reporters", "htmlextra", "--reporter-htmlextra-export", "newman-report.html"]
