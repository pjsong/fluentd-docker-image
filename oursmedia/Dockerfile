FROM fluent/fluentd:latest-onbuild
MAINTAINER your_name <...>
USER fluent
WORKDIR /home/fluent
ENV PATH /home/fluent/.gem/ruby/2.3.0/bin:$PATH
RUN gem install fluent-plugin-secure-forward
EXPOSE 24284
CMD fluentd -c /fluentd/etc/$FLUENTD_CONF -p /fluentd/plugins $FLUENTD_OPT